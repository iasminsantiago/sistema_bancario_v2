# sistema_bancario_v2
Usa como base o projeto [Sistema bancário](https://github.com/iasminsantiago/sistema_bancario)

### Atualizações:
- Separa as funções existentes de saque, depósito e extrato em funções (deixar código mais modularizado)
- Há 2 novas funções:
  - Cadastrar usuário
    - cliente contendo lista com nome, data de nascimento, cpf com números somente e endereço como string contendo logradouro, nro - bairro - cidade/sigla - estado
    - Não pode haver 2 usuários com mesmo cpf.
  - Cadastrar conta corrente: agência, número da conta e usuário. O número da conta é sequencial, inicia em 1. Número da agência é fixo: 0001.
    - O usuário pode ter mais de uma conta, mas uma conta pertence somente a 1 usuário.
    - Para vincular usuário a conta, filtre a lista de usuários buscando CPF na lista
- Saque deve receber argumentos apenas por kwargs
- Depósito deve receber argumentos apenas por posição
- Extrato deve receber argumentos kwargs e args
