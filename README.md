Sistema de Estoque (Terminal)

Este projeto é um sistema de gerenciamento de estoque para ser executado via terminal, desenvolvido em PHP. Ele foi criado como avaliação final para o módulo de Programador de Sistemas do programa Jovem Programador / SENAC SC, sob a orientação do Professor Ricardo.

O objetivo principal é simular as operações básicas de um estoque, com um foco especial na gestão de validade dos produtos e na organização das informações.

>>> Autores

* Gustavo Becker
* Leandro G. S. Fossatti

>>> Funcionalidades

O sistema oferece as seguintes funcionalidades principais:

* Adição de produtos ao estoque.
* Edição de produtos existentes.
* Remoção de produtos do estoque.
* Listagem completa do estoque.
* Listagem específica de produtos fora da validade.
* Listagem de produtos em promoção (aqueles com até 10 dias para vencer).
* Ordenação da listagem principal por código (COD) e validade.
* Verificação automática de validade durante as operações (listagem, adição e edição), baseada na data e hora atual do sistema.

>>> Diferenciais Técnicos

Alguns pontos técnicos que destacam este projeto incluem:

* Verificação de Validade Avançada ⏳: A validade é checada com base na data e hora atual.
* Ao iniciar o programa, produtos vencidos são automaticamente removidos do estoque e adicionados a uma lista de produtos "fora da validade".
* Produtos com até 10 dias para vencer são automaticamente identificados e adicionados a uma lista de "promoção".
* Ordenação Eficiente ↔️: A listagem principal do estoque é ordenada primeiro pelo código do produto e, em seguida, pela validade. Isso é feito utilizando a função uasort() do PHP, que permite uma ordenação     personalizada com base em uma função de callback e o operador "spaceship" (<=>).
* Estrutura de Código Organizada 🗂️: O código utiliza switch case para um controle de fluxo claro do menu principal e apresenta mensagens importantes coloridas no terminal para melhor visualização.
* Cadastro Inteligente ✨: Ao adicionar um produto, o sistema pode solicitar um código para puxar o nome ou não.
* Estrutura de Dados 📦: O estoque é gerenciado através de um array PHP principal com arrays associativos,  o que facilita o acesso e a manipulação dos dados de cada produto (chave => valor).

>>> Como Configurar e Rodar o Projeto

Este é um projeto PHP que roda diretamente no terminal.

1. Pré-requisitos:
    Você precisará ter o **PHP** 🐘 instalado em sua máquina.

2. Clone o Repositório:
    Abra seu terminal ou prompt de comando e clone este repositório:
    git clone https://github.com/GustavoBeckerDev/sistema-estoque-php.git
    cd sistema_estoque

3. Executar o Programa:
    Com o PHP instalado e estando dentro da pasta do projeto, execute o arquivo estoque.php usando o comando PHP:
    php estoque.php
    O programa iniciará no terminal, exibindo o menu de opções.

>>> Melhorias Possíveis

Este projeto pode ser expandido com diversas melhorias no futuro:

* Listagem Filtrada 🔍: Adicionar a capacidade de filtrar a listagem de produtos por nome ou código. Isso seria muito útil para estoques com um grande número de itens.
* Funções Adicionais ➕: Incluir funções para calcular e exibir:
    * Produtos mais caros.
    * O valor total do estoque.
    * Descontos automáticos para produtos em promoção.
* Conexão com Banco de Dados 💾: Atualmente, os dados são armazenados em um array volátil. A integração com um banco de dados (como MySQL ou PostgreSQL) garantiria a persistência das alterações, ou seja, os dados não seriam perdidos ao encerrar o programa.
* Integração com Front-end 🖥️: Desenvolver uma interface gráfica (uma "tela interativa e amigável") para substituir a interação via terminal, proporcionando uma experiência de usuário mais rica.

>>> Contribuições

Sinta-se à vontade para explorar o código, sugerir melhorias ou reportar problemas. Toda contribuição é bem-vinda!
