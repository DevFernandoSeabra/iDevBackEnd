# iDevBackEnd
Projeto de Imersão Developer Back-end com NodeJS e Gemini patrocionado por Alura de 14 a 25 nov/2024.

A idéia é desenvolver o back-end de um site de coleções de postagens de imagens diversas, com foco em criação, leitura, atualização e deleção no que refere-se a postagem da imagem e de sua descrição.

São 5 aulas de mais pura imersão e conhecimento, todas documentadass, testadas e publicadas aqui.

# 4ª AULA - IMPLEMENTANDO ARMAZENAMENTO E UPLOAD DE IMAGENS

**Relatório e documentação;**</p>
<p style="text-align: justify;">
Na aula passada aprendemos a pegar informações ou dados do nosso banco de dados na nossa nuvem "cloud" o mongoDB Atlas. Nessa aula iremos aprender a enviar dados de nossa API para o banco de dados - "vamos enviar posts". Aprendenmos a lidar com os 4 principais verbos HTTPs, são eles; POST (Criar), GET (Ler), PUT ou PATCH(Atualizar), DELETE (Deletar). Desenvolvemos algumas funções e métodos visando as 3 responsabilidades principais, que são sobre: a rota, o controlador (que possui funções de request e response), e o modelo que possui instruções de conexão ao banco de dados.
</p>

**Informações adicionais;**</p>

- Instalamos e Testamos nossa **API RESTful** com a ferramenta **THUNDER CLIENT** de modo a enviar requisições HTTP (GET, POST, PUT, DELETE, PATCH, etc.) diretamente do VS Code para testar APIs. E também o fizemos com outra ferramenta a **POSTMAN** para desktop ambiente Windows 64 bits. Construimos requisições tipo .Json com cabeçalhos personalizados, parâmetros de consulta, corpo de requisição personalizado e autenticação utlizando as ferramentas com auxilio e dentro dos respectivos recursos fornecidos do Thunder Client ou do Postman </p>

- importamos e trabalhamos com **o módulo fs do Node.js** que te permite interagir com o sistema de arquivos, oferecendo operações síncronas e assíncronas para ler, escrever, modificar e excluir arquivos e diretórios. A versão assíncrona é preferida para evitar o bloqueio do evento principal, garantindo melhor desempenho. O módulo fs vai fazer com q nossa API consiga conversar com sistemas de aquivos de nosso computador o servidor local</p>

- instalamos mais uma dependência o **Multer** que é um **middleware para o Node.js** usado para manipulação de uploads de arquivos em aplicativos web, principalmente com o framework Express. Ele facilita o processo de receber e armazenar arquivos enviados por meio de formulários HTML ou APIs.</p>
 
- Manipulamos arquivos do tipo **multipart/form-data** O Multer permite que você trate arquivos enviados com o tipo de conteúdo multipart/form-data, o formato mais comum usado para upload de arquivos via formulários HTML.</p>

- Criamos uma nova pasta na raiz de nosso projeto chamada "uploads" para receber todas as nossas imagens fisícas, com isso a nossa maquina local será um servidor local.</p>

- Aprendemos e trabalhamos com  **template strings** (ou template literals) no JavaScript são uma forma moderna e mais poderosa de trabalhar com strings. Elas foram introduzidas no ECMAScript 6 (ES6) e oferecem várias melhorias em relação às strings tradicionais, como interpolação de variáveis e multi-linhas, entre outras funcionalidades.</p>
Sintaxe das Template Strings:</p>
Template strings são definidas com crase (``) em vez de aspas simples (') ou duplas (").</p>
Exemplo de aplicação código em javaScript:

```javascript
let nome = 'João';
let idade = 25;

// Exemplo básico de template string:
let saudacao = `Olá, meu nome é ${nome} e eu tenho ${idade} anos.`;
console.log(saudacao);  // Saída: "Olá, meu nome é João e eu tenho 25 anos."
```
- No nosso caso, usamos a template strings para juntar dois valores distintos, uma string + uma variável e e seu resultado gera uma nova string que será inserida em uma variavel.</p>
Resumindo: "String Interpolation" (Interpolação de String) é o termo técnico usado para descrever essa prática.</p>
Ao invés de concatenar com o operador +, você insere expressões diretamente dentro da string usando ${}.</p>
Exemplo de código em javaScript:</p>

```javascript
const imagemAtualizada = `uploads/${postcriado.insertedId}.png`
``` 
</p>

- Usamos **Placeholders** em Objetos e Arrays ao trabalhar com dados dinâmicos, onde a estrutura dos dados é definida, mas os valores podem ser preenchidos posteriormente. Que é uma maneira poderosa de tornar seu código mais flexível e dinâmico, seja para manipulação de strings, objetos ou em templates HTML.

- Usamos o **Gemini** IA da google para consulta, complemento e ajuda.</p>

- Usamos comandos **npm / yark**.</p>

- Atualização do arquivo README.md - incrementação de imagens do processo, relatorios e documentação.</p> 

- Criado repositorio iDevBackEnd no **GitHube** e salvo repositório em branch aula_4
</p>

**Imagens do meu projeto neste estagio - aula 3;**

![Instalação do Thunder Client no Visual Studio Code.](imagens/imgA4/tdClient.JPG)</p>
<p>👆 &nbsp; <mark>Instalação do Thunder Client no Visual Studio Code.</mark></p>

![Site do Postman preparando para o baixar.](imagens/imgA4/postman.JPG)</p>
<p>👆 &nbsp; <mark>Site do Postman preparando para o baixar.</mark></p>

![+ uma dependencia instalada no VSCode o "Multer".](imagens/imgA4/multer.JPG)</p>
<p>👆 &nbsp; <mark>+ uma dependencia instalada no VSCode o "Multer".</mark></p>

![Teste de nossa API RESTful módulo GET com a ferramenta de testes  Thunder Client usando url http://localhost:3000/posts.](imagens/imgA4/getTC.JPG)</p>
<p>👆 &nbsp; <mark>Teste de nossa API RESTful módulo GET com a ferramenta de testes  Thunder Client usando url http://localhost:3000/posts.</mark></p>

![Outro teste de nossa API RESTful módulo POST com a ferramenta de testes  Thunder Client usando url http://localhost:3000/posts.](imagens/imgA4/postTC.JPG)</p>
<p>👆 &nbsp; <mark>Outro teste de nossa API RESTful módulo POST com a ferramenta de testes  Thunder Client usando url http://localhost:3000/posts.</mark></p>

![Com o Thunder Client fizemos um novo GET para comprovar que o POST que enviamos anteriormente vide imagem acima, foi devidamente enviado e registrado pelo banco de dados na nuvem o mongoDBAtlas.](imagens/imgA4/getTCBD.JPG)</p>
<p>👆 &nbsp; <mark>Com o Thunder Client fizemos um novo GET para comprovar que o POST que enviamos anteriormente vide imagem acima, foi devidamente enviado e registrado pelo banco de dados na nuvem o mongoDBAtlas.</mark></p>

![Testamos nossa API RESTful com a ferramenta Postman no módulo POST, mas agora gerando PlaceHolders de imagens do tipo .png e a utilizar também a nossa pasta de Uploads como servidor local e usando também a url especifica http://localhost:3000/uploads. Aqui manipulamos arquivos do tipo multipart/form-data.](imagens/imgA4/postUp.JPG)</p>
<p>👆 &nbsp; <mark>Testamos nossa API RESTful com a ferramenta Postman no módulo POST, mas agora gerando PlaceHolders de imagens do tipo .png e a utilizar também a nossa pasta de Uploads como servidor local e usando também a url especifica http://localhost:3000/uploads. Aqui manipulamos arquivos do tipo multipart/form-data</mark></p>


![Complemento da imagem de cima - Site do banco de dados na nuvem mongoDBAtlas indicando que a imagem foi registrado com sucesso o seu insert.](imagens/imgA4/mDBUp.JPG)</p>
<p>👆 &nbsp; <mark>Complemento da imagem de cima - Site do banco de dados na nuvem mongoDBAtlas indicando que a imagem foi registrado com sucesso o seu insert.</mark></p>

![Complemento da imagem de cima - Imagem cat1.png dentro do Visual Studio Code indicando nos que foi salva com sucesso na pasta de uploads dentro de nossa raiz do projeto e de nosso servidor local - nossa maquina.](imagens/imgA4/vscPUp.JPG)</p>
<p>👆 &nbsp; <mark>Complemento da imagem de cima - Imagem cat1.png dentro do Visual Studio Code indicando nos que foi salva com sucesso na pasta de uploads dentro de nossa raiz do projeto e de nosso servidor local - nossa maquina.</mark></p>

![Complemento da imagem de cima - imagem do explorer do windows, exibindo o conteudo da pasta uploads com a imagem salva cat1.png, observe que o Multer nos ajudou a renonear seu ID e deixa-lo comativel com o ID do mongoDBAtlas.](imagens/imgA4/pastUp.JPG)</p>
<p>👆 &nbsp; <mark>Complemento da imagem de cima - imagem do explorer do windows, exibindo o conteudo da pasta uploads com a imagem salva cat1.png, observe que o Multer nos ajudou a renonear seu ID e deixa-lo comativel com o ID do mongoDBAtlas.</mark></p>



◙XXXXXXX

# 3ª AULA - CONECTANDO SUA API AO MONGODB: ESTRUTURA, CONEXÃO E REFATORAÇÃO 

**Relatório e documentação;**</p>
<p style="text-align: justify;">
Nessa aula vamos substituir nossa antiga base de dados o "Array" por nosso BD nas Nuvens, incluir mais uma dependência que é o nosso banco de dados mongoDB Atlas, vamos no site do banco mongoDB Atlas criar e fazer um deploy de nossa database e subir nossas coleções de posts. Vamos pegar todas as nossas informações que estão na cloud e trazer para o nosso projeto. Vamos proteger dados sensíveis criando variáveis de ambiente e o arquivo raiz `.env`. Dentro do arquivo `package.json`, incrementamos o script "dev" dizendo para o node que tem um arquivo de variável de ambiente e seu nome é `.env`.
</p>

<p style="text-align: justify;">
Pela necessidade e evolução de nosso projeto, foi criado um modelo de pastas e arquivos visando as três responsabilidades principais, que são sobre: a rota, o controlador (que possui funções de request e response), e o modelo que possui instruções de conexão ao banco de dados. Criamos para isso uma pasta raiz de nome `src` e, dentro dessa pasta, temos: a pasta `config` e seu arquivo `dbConfig.js`; a pasta `controllers` e seu arquivo `postController.js`; e, por último, a pasta `routes` com o seu arquivo `postsRoutes.js`.
</p>

<p style="text-align: justify;">
Depois, alteramos o código fonte de `server.js`, distribuindo as instruções para cada pasta e arquivo correspondente ao que se trata suas respectivas responsabilidades. Exportamos e importamos funções de um lugar a outro para que essas partes possam se conectar e suas funções serem executadas com êxito.
</p>

**Informações adicionais;**</p>
- Criamos mais uma dependencia **mongoDBAtlas** em nossa API. Configuramos o site e fizemos 3 inserts documents um vedadeiro deploy com dados de nossa coleção de posts.

- Usamos o Gemini IA da google para consulta, complemento e ajuda.</p>

- Aprendemos o que são as palavras chaves async e await dentro de uma função e porque em certos casos, uma vem seguida da outra ao ser declarada.</p>
- Usamos comandos npm / yark.</p>

- Por regras de boa prática o arquivo .gitignore foi alterado impedido que suba no gitHube via comandos no prompt git bash, arquivos como; node_modules, chave-api.txt, mgDB.txt e .env.</p>

- Atualização do arquivo README.md - incrementação de imagens do processo, relatorios e documentação.</p> 

- Criado repositorio iDevBackEnd no GitHube e salvo repositório em branch aula_3
</p>

**Imagens do meu projeto neste estagio - aula 3;**

![Site MongoDBAtlas com coleções de posts criadas.](imagens/imgA3/DB_colecoes.png)</p>
<p>👆 &nbsp; <mark>Site MongoDBAtlas com coleções de posts criadas.</mark></p>

![VSCode arquivo {}package.json - Sript Dev e dependencias.](imagens/imgA3/scriptDev.JPG)</p>
<p>👆 &nbsp; <mark>VSCode arquivo {}package.json - Sript Dev e dependencias.</mark></p>

![localhost:3000/posts resposta do server conectado ao MongoDB nos trazendo as nossas coleções de posts](imagens/imgA3/resServerColecDB.png)</p>
<p>👆 &nbsp; <mark>localhost:3000/posts resposta do server conectado ao MongoDB nos trazendo as nossas coleções de posts</mark></p>


◙XXXXXXX


# 2ª AULA - CRIANDO E ESTRUTURANDO SUA PRIMEIRA API COM GET E BANCO DE DADOS MONGODB ATLAS NA NUVEM.

**Imagens do meu projeto neste estagio - aula 2;**

![Visual Studio Code - codando em node.js + NPM + Expreess + ES6](imagens/tela_VSCode.jpg)</p>
<p>👆 &nbsp; <mark>Visual Studio Code - codando em node.js + NPM + Expreess + ES6.</mark></p>

![Uso do Gemini IA da google como consulta, apoio e criação](imagens/gemini.JPG)</p>
<p>👆 &nbsp; <mark>Uso do Gemini IA da Google como consulta, apoio e criação.</mark></p>

![Resposta do server id1 no Navegador](imagens/server_ID1.JPG)</p>
<p>👆 &nbsp; <mark>Resposta do server id1 no Navegador.*</mark></p>

![Resposta do server id2 no Navegador](imagens/server_ID2.JPG)</p>
<p>👆 &nbsp; <mark>Resposta do server id2 no Navegador.</mark></p>

![Resposta do server id3 no Navegador](imagens/server_ID3.JPG)</p>
<p>👆 &nbsp; <mark>Resposta do server id3 no Navegador.</mark></p>

![Criação da conta do banco de dados MongoDB Atlas(nuvem)](imagens/mongoDB_Atlas.JPG)</p>
<p>👆 &nbsp; <mark>Criação da conta do banco de dados MongoDB Atlas(nuvem).</mark></p>

**Relatório e documentaçao;**</p>
<p style="text-align: justify;">
[No arquivo server.js foi incrementado como uma base de dados uma variavel que recebe uma array de objetos; com id, descrição e imagens], [foi usado a IA Gemini do Google para consulta e criação de imagens e outros], [no código fonte server.js  alteramos info de Rota e incremntação de instancia de API no server], [criada e declarada uma function buscarPostID],[teste de nosso server, teste ok], [Criado conta para acesso ao banco MongoDB_Atlas hospedado na nuvem], [criado a pasta imagens e geradas algumas imagens do processo para arquivo e documentação posteriores], [criado arquivo mgDB.txt com informações sobre dados como username e password e path do banco de dados], [Por regras de boa prática o arquivo .gitignore foi alterado impedido que suba no gitHube via comandos no prompt git bash, arquivos como; node_modules, chave-api.txt e mgDB.txt], [Atualização do arquivo README.md - incrementação de imagens do processo, relatorios e documentação]. [criado repositorio iDevBackEnd no GitHube e salvo repositório em branch aula_2].</p> 

◙XXXXXXX


# 1ª AULA - DESVENDANDO APIS SERVIDORES 

**Relatório / Documentação;**</p>
<p style="text-align: justify;">
[Instalando Nodejs (LTS v.22.11.0) no Windows 10 64bits], [Instalando o Visual Studio Code no windows 10 64 bits], [Testando o Node.JS no terminal CMD do VSCode], [Criação da pasta do projeto "instaslike_back"], [ Instalando NPM e setando a linguagem JavaScript mais moderna ES6 juntamente e automaticamente criou a pasta de  package.json em nosso projeto], [Instalando as depencias como o express v"^4.21.1" via comandos de prompt via npm e junto e automatico a package-lock.json com 65 packages ou dependencias, instalado tbm a pasta node_modules dentro de nosso projeto], [criação do arquivo server.js como nosso servidor, nele  importamos o Express, incrementamos porta 3000 e funções de req request e res response e como respoosta send envia msg in http://localhost:3000/api e após executamos o server para testes e ok testes],[No site da Gemini google, gerando a nossa primeira chave api],[criação do arquivo chave-api.txt], [por boas práticas; criação do arquivo .gitignore para nos comandos do prompt do git bash não subir 2 condições; chave-api.txt e node_modules ], [Iserindo informações de relatório e documentação no arquivo README.md], [criado repositorio iDevBackEnd no GitHube e salvo repositório em branch aula_1]</p> 

◙XXXXXXX

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
