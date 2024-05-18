# Programa de sistema bancário que tem como principal característica a conexão com uma base de dados local em MySQL

O programa se divide em diversas partes, iniciando com a criação de uma classe construtora responsável pela execução das querys que serão utilizadas em cada execução do pgorama juntamente com o bloco de inicizalização do banco de dados.
Feito com tratativa de erros de forma que não gere bugs e erros de execução quando o mesmo for utilizado.

Na base de dados utilizamos 3 tabelas:

* Contas - responsáel pelo armazenamento das contas registradas por meio deo CPF fornecido pelo usuário
* Usuários - responsável por armazenar o CPF do usuário juntamente com seus dados pessoais como endereço, idade, data de nascimento e nome
* Transações - responsável po armazenar todo o giro de informações que ocorrem entre as contas, será usada para posterior apoio na apresentação do extrato exigido pelo usuário e por fim para controle de execução.

Todas as informações são executadas por métodos dentro da classe de execução chamada AppBancodeDados que inicializa a conexão com o database no MySQL e gera todos os métodos que executam as querys quando fornecida pelo usuário todas as informações.

Convido-os para olhar o código e apontar melhorias que possam ser enriquecedoras para meu conhecimento.

Ainda deixo aqui melhorias que podem ocorrer que é a tratativa de erros em cada fornecimento de informação pelo usuário, afim de evitar erros dentro do bloco de execução dentro da classe main.
