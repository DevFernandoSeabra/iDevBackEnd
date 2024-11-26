# iDevBackEnd
Projeto de Imersão Developer Back-end com NodeJS e Gemini patrocionado por Alura de 14 a 25 nov/2024.

# 3ª AULA - CONECTANDO SUA API AO MONGODB: ESTRUTURA, CONEXÃO E REFATORAÇÃO 

<<<<<<< HEAD

**Relatório e documentação;**</p>
Nessa aula vamos substituir nossa antiga base de dados o "Array" por nosso BD nas Nuvens, incluir mais uma dependencia que é o nosso banco de dados mongoDB, vamos no site do banco mongoDB Atlas criar e fazer um deploy de nossa database e subir nossas coleções de posts, vamos pegar todas as nossas informções que estão na cloud e trazer para o nosso projeto, vamos proteger dados sensiveis criando variáveis de ambiente e arquivo raiz .env, dentro do arquivo package.json icrementamos a script "dev" dizendo para o node que tem um arquivo de variavel de ambiente e seu nome é .env, pela necessidade e evolução de nosso projeto foi criado um modelo de pastas e arquivos visando as 3 responsabilidades prinicipais que são sobre; a rota, o controlador (que possui funções de request e response) e o modelo q possui instruções de conexão ao banco de dados, criamos para isso uma pasta raiz de nome src e dentro dessa pasta temos; a pasta config e seu arquivo dbConfig.js, temos a pasta controllers e seu arquivo postController.js e por ultimo a pasta routes com o seu arquivo postsRoutes.js, depois alteramos o código fonte de server.js distribuindo as instruções para cada pasta e arquivo correspondente ao que se trata as suas respectivas responsabilidades, exportamos e importamos funções de um lugar a outro para que essas partes possam ser conectar e suas fuções serem executadas com êxito.  

**Informações adicionais;**</p>
Usamos o Gemini IA da google para consulta, complemento e ajuda.
Aprendemos o que são as palavras chaves async e await dentro de uma função e porque em certos casos, uma vem seguida da outra ao ser declarada.
Usamos comandos npm / yark.
Por regras de boa prática o arquivo .gitignore foi alterado impedido que suba no gitHube via comandos no prompt git bash, arquivos como; node_modules, chave-api.txt, mgDB.txt e .env. Atualização do arquivo README.md - incrementação de imagens do processo, relatorios e documentação. Criado repositorio iDevBackEnd no GitHube e salvo repositório em branch aula_3


**Imagens do meu projeto neste estagio - aula 3;**

![Site MongoDBAtlas com coleções de posts criadas.](imagens/imgA3/DB_colecoes.png)</p>
👆*Site MongoDBAtlas com coleções de posts criadas.*</p>

![VSCode arquivo {}package.json - Sript Dev e dependencias.](imagens/imgA3/scriptDev.JPG)</p>
👆*VSCode arquivo {}package.json - Sript Dev e dependencias.*</p>

![localhost:3000/posts resposta do server conectado ao MongoDB nos trazendo as nossas coleções de posts](imagens/imgA3/resServerColecDB.png)</p>
👆*localhost:3000/posts resposta do server conectado ao MongoDB nos trazendo as nossas coleções de posts*</p>


◙XXXXXXX
=======
>>>>>>> 

# 2ª AULA - CRIANDO E ESTRUTURANDO SUA PRIMEIRA API COM GET E BANCO DE DADOS MONGODB ATLAS NA NUVEM.
<<<<<<< HEAD

**Imagens do meu projeto neste estagio - aula 2;**

![Visual Studio Code - codando em node.js + NPM + Expreess + ES6](imagens/tela_VSCode.jpg)</p>
👆*Visual Studio Code - codando em node.js + NPM + Expreess + ES6.*</p>

![Uso do Gemini IA da google como consulta, apoio e criação](imagens/gemini.JPG)</p>
👆*Uso do Gemini IA da google como consulta, apoio e criação.*</p>

![Resposta do server id1 no Navegador](imagens/server_ID1.JPG)</p>
👆*Resposta do server id1 no Navegador.*</p>

![Resposta do server id2 no Navegador](imagens/server_ID2.JPG)</p>
👆*Resposta do server id2 no Navegador.*</p>

![Resposta do server id3 no Navegador](imagens/server_ID3.JPG)</p>
👆*Resposta do server id3 no Navegador.*</p>

![Criação da conta do banco de dados MongoDB Atlas(nuvem)](imagens/mongoDB_Atlas.JPG)</p>
👆*Criação da conta do banco de dados MongoDB Atlas(nuvem).*</p>

**Relatório e documentaçao;**</p>
[No arquivo server.js foi incrementado como uma base de dados uma variavel que recebe uma array de objetos; com id, descrição e imagens], [foi usado a IA Gemini do Google para consulta e criação de imagens e outros], [no código fonte server.js  alteramos info de Rota e incremntação de instancia de API no server], [criada e declarada uma function buscarPostID],[teste de nosso server, teste ok], [Criado conta para acesso ao banco MongoDB_Atlas hospedado na nuvem], [criado a pasta imagens e geradas algumas imagens do processo para arquivo e documentação posteriores], [criado arquivo mgDB.txt com informações sobre dados como username e password e path do banco de dados], [Por regras de boa prática o arquivo .gitignore foi alterado impedido que suba no gitHube via comandos no prompt git bash, arquivos como; node_modules, chave-api.txt e mgDB.txt], [Atualização do arquivo README.md - incrementação de imagens do processo, relatorios e documentação]. [criado repositorio iDevBackEnd no GitHube e salvo repositório em branch aula_2] 

◙XXXXXXX
=======
>>>>>>> 

# 1ª AULA - DESVENDANDO APIS SERVIDORES 
<<<<<<< HEAD

**Relatório / Documentação;**</p>
[Instalando Nodejs (LTS v.22.11.0) no Windows 10 64bits], [Instalando o Visual Studio Code no windows 10 64 bits], [Testando o Node.JS no terminal CMD do VSCode], [Criação da pasta do projeto "instaslike_back"], [ Instalando NPM e setando a linguagem JavaScript mais moderna ES6 juntamente e automaticamente criou a pasta de  package.json em nosso projeto], [Instalando as depencias como o express v"^4.21.1" via comandos de prompt via npm e junto e automatico a package-lock.json com 65 packages ou dependencias, instalado tbm a pasta node_modules dentro de nosso projeto], [criação do arquivo server.js como nosso servidor, nele  importamos o Express, incrementamos porta 3000 e funções de req request e res response e como respoosta send envia msg in http://localhost:3000/api e após executamos o server para testes e ok testes],[No site da Gemini google, gerando a nossa primeira chave api],[criação do arquivo chave-api.txt], [por boas práticas; criação do arquivo .gitignore para nos comandos do prompt do git bash não subir 2 condições; chave-api.txt e node_modules ], [Iserindo informações de relatório e documentação no arquivo README.md], [criado repositorio iDevBackEnd no GitHube e salvo repositório em branch aula_1] 

◙XXXXXXX
=======
>>>>>>> 


- 👋 Hi, I’m @DevFernandoSeabra
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...


<!---
DevFernandoSeabra/DevFernandoSeabra is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
