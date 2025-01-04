# Repositório criado para armazenar o código da API de autenticação com banco de dados.
dia 31/12
https://www.notion.so/Python-dia-31-12-16dbc5c3824d80009875d546d69e26f6
Banco de dados é usado para gerenciamento armazenamento e troca de informações, sendo uma memoria não volatil;
FlaskSQLAlchmey, é usado para fazer a ponte entre do flask e o nosso banco de dados, permitindo acesso, alteração, mapeamento de objetos relacionais, também tem o auxilio do ORM, onde fazemos uma troca de banco de dados facilmente, porém ficamos dependente dele.
Nos vimos a SECRET_KEY, onde é bem parecida com o KEY_STRING, vimos também SQLALCHEMY_DATA_BASE, onde colocamos o caminho do nosso banco de dados, vimos a função Model, onde o flaskalchemy reconhece ele como algo mapeável. Vimos os tipos de textos em uma data base, e sua colunas =(Column), flask shell e sua execução do banco de dados. EVITAR IMPORTAÇÕES CIRCULARES.

dia 02/01
https://www.notion.so/Python-dia-02-01-16fbc5c3824d80e4b0a9f550cc302025
Hoje vimos, mais sobre autenticação de login em flask_login/
fornece uma seção de gerenciamento de login, logout e lembrar a sessão(cookies). Necessitando de um de banco de dados para armazenar os cookies. Rotas que envolve requisição de autenticação é recomendável que seja feita com methods POST. 
Fazenda a conversão do data em uma rota; data = request.json (request é uma função do flask.)
com query em flask, conseguimos fazer get(), pegando apenas o autenticador primário(id), ou o filter() pegando de forma geral.
flask_login;
login_user(recebe um usuário), faz a autenticação direta com o banco de dados.
current_user(is_authenticated), nos trás mais informações do usuário logado.
user_loader(), salva a sessão em cookies.
logout()GET, desconecta da sessão.
@login_required, é um decorator que nos deixa fazer execução caso estejamos logados.

dia 03/01
https://www.notion.so/dia-03-01-and-Python-170bc5c3824d8054bd3ff6945d4a207d
Hoje vimos, sobre a criação de rotas, PUT, onde devemos sim preservar mais a atualização de senha, podendo usar até mesmo alguns hashs;
query, faz uma busca de chaves em nosso banco de dados, podendo chamar get para pegar a chave.
request.json, sempre será oq o usuário nos mandar...
Todas as vezes que formos mexer de forma geral em um banco de dados, precisamos dar o commit(), para que a alteração seja feita.
current_user.id, é o id do nosso usuário atual.