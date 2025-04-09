#Query-Builder-NodeJs.
 
 Projeto de Query Builders para abstrair o código SQL e manipular o banco de dados utilizando os Métodos: inserir, selecionar, atualizar dados e também como versionar o banco de dados com Migrations e popular dados com Seeds.

- Contexto: Um Query Builder é uma ferramenta que permite construir instruções SQL independentemente do banco de dados utilizado. Ele abstrai a complexidade do SQL, permitindo o uso de métodos para selecionar, inserir e atualizar dados.
- Alcançado: Uma API que conecta os módulos aos cursos colocando em prática os conceitos do SQL de "Relacionamento Muito para Muitos (N:M)"

- Foi desenvolvido com SQL Query Builder Knex.js.

____________________________________________________________________________________________________________________________________________________________________________________________________________________
____________________________________________________________________________________________________________________________________________________________________________________________________________________
- Migrations:
  
- um recurso importante para definir a estrutura das tabelas em um banco de dados porque permitem criar, modificar e gerenciar mudanças no banco de dados ao longo do tempo, possibilitando o versionamento do banco de dados
- criar a primeira migration utilizando o Knex na aplicação é necessário configurar um script para lidar com arquivos TypeScript, já que o Knex por padrão lida com arquivos JavaScript.
- criar uma tabela no banco de dados utilizando o Knex com as funções up e down de uma migration, onde up é responsável por criar a tabela e down por desfazê-la e definir tipos de dados e restrições.
- criar uma nova migration para adicionar uma coluna em uma tabela existente no banco de dados ou desfazer de uma migration.

____________________________________________________________________________________________________________________________________________________________________________________________________________________
____________________________________________________________________________________________________________________________________________________________________________________________________________________
- Manipulações:
  
- Método Insert para inserir dados na tabela.
- Método RAW para escrever SQL no Query Builder, permitindo flexibilidade. inserir dados em uma tabela usando SQL, com a opção de concatenar valores.
- Método Select para listar os dados na tabela com ou sem parâmetros.
- Método Update para atualizar os dados recuperando o ID a ser atualizado e o nome a ser modificado no corpo da requisição filtrando com WHERE.
- Método Delete para remover os registros.
- Utilizado o recurso de SEED com o Knex para popular tabelas com vários registros de uma vez.
____________________________________________________________________________________________________________________________________________________________________________________________________________________
____________________________________________________________________________________________________________________________________________________________________________________________________________________
- Relacionamentos:
  
- criada uma nova tabela chamada "course-modules" para armazenar os módulos de um curso, estabelecendo um relacionamento com a tabela de cursos.
- utilizado o conceito de chave estrangeira(foreign_key) para vincular os módulos aos cursos.
- Conectado duas tabelas usando o join: criar uma nova requisição, adicionar parâmetros e realizar consultas entre tabelas, assim, podendo retornar dados específicos de cada uma.
- exibido informações de tabelas relacionadas, facilitando a visualização dos dados.
____________________________________________________________________________________________________________________________________________________________________________________________________________________
____________________________________________________________________________________________________________________________________________________________________________________________________________________
-------> Ferramentas:

- visualizar um banco de dados SQLite utilizando o Beekeeper:
![telabeekeeper](https://github.com/user-attachments/assets/33fb1dd3-d258-41f0-a378-df64ad117590)

- o uso do Insomnia para testar as requisições:
![telainsomnia](https://github.com/user-attachments/assets/f5e9bc6b-2da6-453e-b680-1f786a2a9a68)

____________________________________________________________________________________________________________________________________________________________________________________________________________________
____________________________________________________________________________________________________________________________________________________________________________________________________________________

Tecnologias: TYPESCRIPT. NODEJS.
