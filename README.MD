# Repositório criado para armazenar o código da API de autenticação com banco de dados.
dia 31/12
https://www.notion.so/Python-dia-31-12-16dbc5c3824d80009875d546d69e26f6
Banco de dados é usado para gerenciamento armazenamento e troca de informações, sendo uma memoria não volatil;
FlaskSQLAlchmey, é usado para fazer a ponte entre do flask e o nosso banco de dados, permitindo acesso, alteração, mapeamento de objetos relacionais, também tem o auxilio do ORM, onde fazemos uma troca de banco de dados facilmente, porém ficamos dependente dele.
Nos vimos a SECRET_KEY, onde é bem parecida com o KEY_STRING, vimos também SQLALCHEMY_DATA_BASE, onde colocamos o caminho do nosso banco de dados, vimos a função Model, onde o flaskalchemy reconhece ele como algo mapeável. Vimos os tipos de textos em uma data base, e sua colunas =(Column), flask shell e sua execução do banco de dados. EVITAR IMPORTAÇÕES CIRCULARES.