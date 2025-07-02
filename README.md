# MC536: Segunda Avaliação
Segundo projeto para a matéria MC536 ministrada no 1º semestre de 2025 pelo professor Breno Bernard Nicolau de França, Instituto de Computação da Universidade Estadual de Campinas (UNICAMP).
Este projeto é autoria de:
  - [Daniel Baltieri Ismael (247855)](https://github.com/DBisma)
  - [Gustavo Costa Salles Silva (198487)](https://github.com/gu-css)
  - [João Emílio Ferreira (247184)](https://github.com/Gmilho/)

## Objetivos e Decisões
O objetivo desta segunda avaliação foi transferir para um novo banco de dados os _datasets_ utilizados para a construção do banco de dados da primeira avaliação. Para isso, foi escolhido o **[duckDB](https://duckdb.org/)**, que proporciona análises e estáticas rápidas sobre um grande volumes de dados e é especialmente eficiente quando inserções de dados são pouco frequentes. Dentre outras vantagens deste banco de dados:
   * As consultas podem ser realizadas diretamente por Python, bastando apenas importar a biblioteca do duckDB;
   * Por conta de ser um banco colunar, há uma maior compressão dos dados, diminuindo o tamanho necessário para armazenar o banco;
   * Por conta disso, o banco pode até tornar-se portável, possibilitando consultas no banco hospedado num _notebook_;
   * O banco de dados é _in-memory_: Dados relevantes em processo são carregados na memória _RAM_ conforme necessário, tornando o acesso muito mais rápido do que é o caso com bancos armazenados em disco rígido;
   * Transações consistentes e seguras garantidas pelas propriedades _ACID_; na ocasião de uma transação falhar, o sistema faz um _rollback_. 

## Obtendo Dependências e Executando
Este projeto depende de [Python 3](https://www.python.org/), [Pip](https://pypi.org/project/pip/), [Jupyter](https://jupyter.org/) e [DuckDB](https://duckdb.org/).





# TODO
O banco foi reduzido a apenas uma tabela:  
![modelo lógico](proj2logico.drawio.png)



