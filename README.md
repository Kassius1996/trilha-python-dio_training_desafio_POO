# trilha-python-dio_training_desafio_POO
Treinamento/Contribuição

💳 Sistema Bancário em Python (Orientado a Objetos)

Aplicação de linha de comando que simula um sistema bancário simples, implementado com Python e Programação Orientada a Objetos (POO).
Permite cadastrar clientes, criar contas correntes, realizar depósitos, saques, consultar extratos e listar contas.

⚙️ Funcionalidades

Criar clientes (Pessoa Física) com CPF único.

Criar contas correntes vinculadas a clientes.

Depósitos e saques com regras de limite.

Controle de histórico de transações (com data/hora).

Extrato de cada conta.

Listagem de todas as contas cadastradas.

Menu interativo no terminal.

📂 Estrutura de Classes

Cliente → classe base com endereço e lista de contas.

PessoaFisica → herda de Cliente, inclui nome, CPF e data de nascimento.

Conta → base para contas bancárias (saldo, número, agência, cliente, histórico).

ContaCorrente → herda de Conta, adiciona limite de valor e limite de saques.

Historico → armazena transações (valor, tipo, data).

Transacao (abstract) → classe abstrata para modelar Saque e Deposito.

Saque → operação de saque com regras de limite e saldo.

Deposito → operação de depósito.

🖥️ Menu Principal

================ MENU ================
[d] Depositar
[s] Sacar
[e] Extrato
[nc] Nova conta
[lc] Listar contas
[nu] Novo usuário
[q] Sair

▶️ Como Executar

Clone este repositório:

git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio


Certifique-se de ter Python 3.10+ instalado.

Execute o programa:

python sistema_bancario.py

📌 Exemplo de Uso
Informe o CPF (somente número): 12345678900
Informe o nome completo: João da Silva
Informe a data de nascimento (dd-mm-aaaa): 10-05-1985
Informe o endereço: Rua A, 123 - Centro - São Paulo/SP

=== Cliente criado com sucesso! ===

Informe o CPF do cliente: 12345678900
=== Conta criada com sucesso! ===

Informe o CPF do cliente: 12345678900
Informe o valor do depósito: 500
=== Depósito realizado com sucesso! ===

================ EXTRATO ================
Deposito:
    R$ 500.00
    31-08-2025 19:22:45

Saldo:
    R$ 500.00
==========================================

🛠️ Tecnologias Utilizadas

Python 3.10+

Programação Orientada a Objetos (POO)

Módulo abc (classes abstratas)

Módulo datetime (datas e horários)

📈 Possíveis Melhorias

Persistência em arquivo JSON ou banco de dados.

Uso de Decimal para valores monetários.

Limite de saques diários (não apenas total).

Interface gráfica (Tkinter, PyQt) ou API (Flask/FastAPI).

Testes automatizados com pytest.

📄 Licença

Este projeto é distribuído sob a licença MIT.
Sinta-se livre para usar, modificar e compartilhar.
