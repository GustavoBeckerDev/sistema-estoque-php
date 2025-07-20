Sistema de Estoque (Terminal)

Este projeto é um sistema de gerenciamento de estoque para ser executado via terminal, desenvolvido em PHP. Ele foi criado como avaliação final para o módulo de Programador de Sistemas do programa Jovem Programador / SENAC SC, sob a orientação do Professor Ricardo.

O objetivo principal é simular as operações básicas de um estoque, com um foco especial na gestão de validade dos produtos e na organização das informações.

>>> Autores

* Gustavo Becker
* Leandro G. S. Fossatti

>>> Funcionalidades

O sistema oferece as seguintes funcionalidades principais:

* [cite_start]Adição de produtos ao estoque. [cite: 8]
* [cite_start]Edição de produtos existentes. [cite: 9]
* [cite_start]Remoção de produtos do estoque. [cite: 10]
* [cite_start]Listagem completa do estoque. [cite: 11]
* [cite_start]Listagem específica de produtos fora da validade. [cite: 12]
* [cite_start]Listagem de produtos em promoção (aqueles com até 10 dias para vencer). [cite: 13]
* [cite_start]Ordenação da listagem principal por código (COD) e validade. [cite: 14]
* [cite_start]Verificação automática de validade durante as operações (listagem, adição e edição), baseada na data e hora atual do sistema. [cite: 15]

>>> Diferenciais Técnicos

Alguns pontos técnicos que destacam este projeto incluem:

* [cite_start]Verificação de Validade Avançada ⏳: A validade é checada com base na data e hora atual. [cite: 19]
    * [cite_start]Ao iniciar o programa, produtos vencidos são automaticamente removidos do estoque e adicionados a uma lista de produtos "fora da validade". [cite: 21, 22]
    * [cite_start]Produtos com até 10 dias para vencer são automaticamente identificados e adicionados a uma lista de "promoção". [cite: 23]
* [cite_start]Ordenação Eficiente ↔️: A listagem principal do estoque é ordenada primeiro pelo código do produto e, em seguida, pela validade. [cite: 27] [cite_start]Isso é feito utilizando a função uasort() do PHP, que permite uma ordenação personalizada com base em uma função de callback e o operador "spaceship" (<=>). [cite: 28]
* [cite_start]Estrutura de Código Organizada 🗂️: O código utiliza switch case para um controle de fluxo claro do menu principal [cite: 30] [cite_start]e apresenta mensagens importantes coloridas no terminal para melhor visualização. [cite: 31]
* [cite_start]Cadastro Inteligente ✨: Ao adicionar um produto, o sistema pode solicitar um código para puxar o nome ou não. [cite: 32]
* [cite_start]Estrutura de Dados 📦: O estoque é gerenciado através de um array PHP principal com arrays associativos, [cite: 33] o que facilita o acesso e a manipulação dos dados de cada produto (chave => valor).

>>> Como Configurar e Rodar o Projeto

Este é um projeto PHP que roda diretamente no terminal.

1. Pré-requisitos:
    Você precisará ter o **PHP** 🐘 instalado em sua máquina.

2. Clone o Repositório:
    Abra seu terminal ou prompt de comando e clone este repositório:
    git clone https://github.com/seu-usuario/sistema_estoque.git
    cd sistema_estoque

3. Executar o Programa:
    Com o PHP instalado e estando dentro da pasta do projeto, execute o arquivo estoque.php usando o comando PHP:
    php estoque.php
    O programa iniciará no terminal, exibindo o menu de opções.

>>> Melhorias Possíveis

Este projeto pode ser expandido com diversas melhorias no futuro:

* [cite_start]Listagem Filtrada 🔍: Adicionar a capacidade de filtrar a listagem de produtos por nome ou código. [cite: 37] [cite_start]Isso seria muito útil para estoques com um grande número de itens. [cite: 38]
* Funções Adicionais ➕: Incluir funções para calcular e exibir:
    * [cite_start]Produtos mais caros. [cite: 40]
    * [cite_start]O valor total do estoque. [cite: 41]
    * [cite_start]Descontos automáticos para produtos em promoção. [cite: 42]
* Conexão com Banco de Dados 💾: Atualmente, os dados são armazenados em um array volátil. [cite_start]A integração com um banco de dados (como MySQL ou PostgreSQL) garantiria a persistência das alterações, ou seja, os dados não seriam perdidos ao encerrar o programa. [cite: 43, 44]
* [cite_start]Integração com Front-end 🖥️: Desenvolver uma interface gráfica (uma "tela interativa e amigável") para substituir a interação via terminal, proporcionando uma experiência de usuário mais rica. [cite: 45, 46]

>>> Contribuições

Sinta-se à vontade para explorar o código, sugerir melhorias ou reportar problemas. Toda contribuição é bem-vinda!
