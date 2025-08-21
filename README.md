# gitegithub.md

# O que é Git?
•	Git é um sistema de controle de versão distribuído, criado por Linus Torvalds em 2005 para o desenvolvimento do kernel do Linux. Ele permite que desenvolvedores (ou qualquer pessoa trabalhando com arquivos de texto, como código fonte) rastreiem mudanças em arquivos ao longo do tempo. 

## Funções principais do Git:
 
- Rastreamento de versões: Registra histórico de alterações em arquivos, permitindo voltar a versões anteriores se necessário.
- Trabalho colaborativo local: 
Permite criar branches (ramificações) para desenvolver features separadamente, mesclar (merge) mudanças e resolver conflitos.
-	Distribuído: 
Cada usuário tem uma cópia completa do repositório localmente, o que significa que você pode trabalhar offline e sincronizar depois.
-	Eficiência: 
É rápido e leve, otimizado para projetos grandes.
- Git é uma ferramenta de linha de comando (embora existam interfaces gráficas como Git GUI ou integrações em editores como VS Code), e é gratuito e open-source. Você instala no seu computador e usa comandos como git init, git add, git commit, git push, etc.

# O que é github?
- Github é uma plataforma web baseada em Git, lançada em 2008 e adquirida pela Microsoft em 2018. Ela atua como um serviço de hospedagem para repositórios Git, facilitando a colaboração online entre equipes.
Funções principais do github:
-	Hospedagem de repositórios: 
Armazena repositórios Git na nuvem, permitindo acesso remoto e backup.
-	Colaboração remota:
Recursos como pull requests (para revisar e mesclar código), issues (para rastrear bugs ou tarefas), forks (cópias de repositórios para contribuições) e wikis.

-	Integrações e ferramentas sociais: 
Suporte a CI/CD (integração contínua), github Actions para automação, e features sociais como stars, watches e discussões.
-	Comunidade e open-source: 
Milhões de projetos open-source são hospedados lá, facilitando contribuições globais.

- Github é acessível via navegador ou apps, e oferece planos gratuitos (para repositórios públicos) e pagos (para privados ou features avançadas). Não é obrigatório usar github com Git; você pode usar Git sozinho ou com outras plataformas como gitlab ou Bitbucket.

## Protocolos de rede e comunicação (HTTP, HTTPS, websockets, FTP, SSH, SSL)

## HTTP (Hypertext Transfer Protocol)
-	O que é: Protocolo fundamental para a World Wide Web. Ele define como os clientes (navegadores) e servidores web se comunicam.

###	Para que serve:
- É usado para transferir páginas web (HTML), imagens, scripts e outros recursos. É a base da navegação na internet como a conhecemos.

## HTTPS (Hypertext Transfer Protocol Secure)
-	O que é: Versão segura do HTTP. Ele usa criptografia para proteger os dados em trânsito.

###	Para que serve: 
- Garante a confidencialidade e integridade dos dados, sendo essencial para transações financeiras, login em sites e qualquer informação sensível.

###	Porta Padrão: 
- Porta 443.

## Websockets
###	O que é: 
- Protocolo que permite uma comunicação full-duplex (bidirecional) entre um cliente e um servidor através de uma única conexão TCP de longa duração.

###	Para que serve: 
- Ideal para aplicações em tempo real, como chats, jogos online, notificações de bolsa de valores ou qualquer sistema que precise de atualizações contínuas sem que o cliente precise fazer uma nova requisição.

### Porta Padrão: 
- Não tem uma porta padrão única, mas é comum usar a porta 80 (HTTP) ou 443 (HTTPS) para a conexão inicial.

## FTP (File Transfer Protocol)
###	O que é: 
Protocolo para a transferência de arquivos entre um cliente e um servidor.

### Para que serve: 
- Usado para fazer upload e download de arquivos grandes. Por exemplo, para publicar arquivos de um site em um servidor web.

### Portas Padrão: 
- Portas 20 e 21. A porta 21 é para controle de comandos, e a porta 20 é para a transferência de dados.

## SSH (Secure Shell)
###	O que é: 
- Protocolo de rede criptografado para operar serviços de rede de forma segura em redes não seguras.

###	Para que serve: 
- Usado para acesso remoto a servidores (geralmente via linha de comando), gerenciamento de servidores, transferência segura de arquivos, etc.

### Porta Padrão: 
- Porta 22.

## SSL/TLS (Secure Sockets Layer / Transport Layer Security)
### O que é: 
- SSL (agora obsoleto) e seu sucessor, TLS, são protocolos criptográficos que fornecem segurança de comunicação na internet.

###	Para que serve: 
- Usados para criptografar a comunicação de outros protocolos, como o HTTP (criando o HTTPS). Eles garantem que os dados trocados entre um cliente e um servidor não possam ser interceptados ou lidos por terceiros.

## Arquitetura cliente-servidor.
-	arquitetura cliente-servidor é um modelo de computação distribuída. Um cliente (como seu navegador web ou um aplicativo de celular) solicita um serviço ou recurso de um servidor, que por sua vez, processa a solicitação e envia uma resposta.

###	Cliente:
- Faz a requisição. Pense no seu navegador pedindo uma página web.

###	Servidor: 
- Fornece o serviço ou recurso. Pense no computador que armazena os arquivos do site e os envia para o seu navegador.


## Funcionamento do DNS e de proxies.
-	DNS (Domain Name System): É um sistema hierárquico e distribuído que traduz nomes de domínio legíveis por humanos (como www.example.com) em endereços IP numéricos (como 192.168.1.1) que os computadores usam para se conectar. 
Funciona assim:
- O usuário digita um domínio no navegador.
- O resolvedor DNS local (no dispositivo ou roteador) consulta um servidor DNS recursivo.
- Se não cached, o recursivo consulta servidores raiz, depois TLD (Top-Level Domain, como .com) e autoritativos do domínio.
-	O IP é retornado e cached para acessos futuros. 
Proxies: São intermediários entre cliente e servidor que encaminham requisições. Tipos incluem:
- Forward Proxy: Cliente usa para acessar a internet anonimamente ou filtrar conteúdo; esconde o IP do cliente. 

- Reverse Proxy: Servidor usa para balancear carga, cache ou segurança; esconde o IP do servidor.

- DNS Proxy: Encaminha consultas DNS para outro servidor, melhorando performance via cache. 

- Funcionam interceptando requisições, processando (ex: caching) e encaminhando, com usos em privacidade, otimização e segurança
- Diferenças entre HTTP e HTTPS.
- Segurança: HTTP transmite dados em texto plano, vulnerável a interceptações; HTTPS usa TLS/SSL para criptografar, protegendo contra eavesdropping e man-in-the-middle. 

- Porta: HTTP usa 80; HTTPS usa 443. 

- Certificados: HTTPS requer certificado digital para autenticação; HTTP não. 

- Performance: HTTPS é ligeiramente mais lento devido à criptografia, mas otimizações modernas minimizam isso. 

- Uso: HTTP para sites não sensíveis; HTTPS obrigatório para e-commerce, logins e SEO (Google prioriza). 
 

## Principais categorias de códigos HTTP (2xx, 4xx, 5xx) e os verbos de requisição.

* São códigos de status que o servidor envia ao cliente na resposta, indicando o resultado da requisição.

-	2xx (Sucesso): A requisição foi recebida, entendida e aceita com sucesso. Ex: 200 OK (requisição bem-sucedida).

- 4xx (Erro do Cliente): O cliente cometeu um erro. Ex: 404 Not Found (o recurso solicitado não existe), 401 Unauthorized (não autorizado).

- 5xx (Erro do Servidor): O servidor falhou ao processar uma requisição válida. Ex: 500 Internal Server Error (um erro genérico no servidor), 503 Service Unavailable (servidor temporariamente indisponível).

* Verbos de Requisição
São métodos que indicam a ação que o cliente quer realizar no servidor.

-	GET: Solicita dados de um recurso específico.

-	POST: Envia dados para o servidor para criar um novo recurso.

-	PUT: Envia dados para atualizar um recurso existente.

- DELETE: Remove um recurso específico.


## Protocolos de Rede e Comunicação

### O que são?

- Protocolos de rede são conjuntos de regras e padrões que permitem a comunicação e a troca de dados entre dispositivos em uma rede. Eles garantem que todos os computadores, servidores e outros dispositivos "falem a mesma língua", entendendo como os dados são formatados, transmitidos e recebidos.

## HTTP (Hypertext Transfer Protocol)

### O que é: 
- Protocolo fundamental para a World Wide Web. Ele define como os clientes (navegadores) e servidores web se comunicam.

### Para que serve: 
- É usado para transferir páginas web (HTML), imagens, scripts e outros recursos. É a base da navegação na internet como a conhecemos.

### Porta Padrão:
- Porta 80.

## HTTPS (Hypertext Transfer Protocol Secure)
### O que é:
- Versão segura do HTTP. Ele usa criptografia para proteger os dados em trânsito.

### Para que serve: 
- Garante a confidencialidade e integridade dos dados, sendo essencial para transações financeiras, login em sites e qualquer informação sensível.

### Porta Padrão:
- Porta 443.

## Websockets
### O que é: 
- Protocolo que permite uma comunicação full-duplex (bidirecional) entre um cliente e um servidor através de uma única conexão TCP de longa duração.

### Para que serve: 
- Ideal para aplicações em tempo real, como chats, jogos online, notificações de bolsa de valores ou qualquer sistema que precise de atualizações contínuas sem que o cliente precise fazer uma nova requisição.

### Porta Padrão: 
- Não tem uma porta padrão única, mas é comum usar a porta 80 (HTTP) ou 443 (HTTPS) para a conexão inicial.

## FTP (File Transfer Protocol)
### O que é: 
- Protocolo para a transferência de arquivos entre um cliente e um servidor.

### Para que serve: 
- Usado para fazer upload e download de arquivos grandes. Por exemplo, para publicar arquivos de um site em um servidor web.

### Portas Padrão: 
- Portas 20 e 21. A porta 21 é para controle de comandos, e a porta 20 é para a transferência de dados.

## SSH (Secure Shell)
### O que é: 
- Protocolo de rede criptografado para operar serviços de rede de forma segura em redes não seguras.

### Para que serve: 
- Usado para acesso remoto a servidores (geralmente via linha de comando), gerenciamento de servidores, transferência segura de arquivos, etc.

### Porta Padrão: 
- Porta 22.

## SSL/TLS (Secure Sockets Layer / Transport Layer Security)

### O que é: 
- SSL (agora obsoleto) e seu sucessor, TLS, são protocolos criptográficos que fornecem segurança de comunicação na internet.

### Para que serve:
- Usados para criptografar a comunicação de outros protocolos, como o HTTP (criando o HTTPS). Eles garantem que os dados trocados entre um cliente e um servidor não possam ser interceptados ou lidos por terceiros.

## Arquitetura Cliente-Servidor

* A arquitetura cliente-servidor é um modelo de computação distribuída. Um cliente (como seu navegador web ou um aplicativo de celular) solicita um serviço ou recurso de um servidor, que por sua vez, processa a solicitação e envia uma resposta.

### Cliente: 
- Faz a requisição. Pense no seu navegador pedindo uma página web.

### Servidor: 
- Fornece o serviço ou recurso. Pense no computador que armazena os arquivos do site e os envia para o seu navegador.

## Funcionamento de DNS e Proxies

### DNS (Domain Name System)

### Funcionamento: 
- Pense no DNS como uma grande agenda telefônica da internet. Quando você digita um nome de domínio como www.google.com no seu navegador, o DNS traduz esse nome em um endereço IP (ex: 142.250.187.164). Seu navegador então usa esse IP para encontrar e se conectar ao servidor correto.

## Proxies
### O que é:
- Um servidor intermediário que atua como um "ponte" entre um cliente e outro servidor.

### Funcionamento: 
- Quando você usa um proxy, sua requisição não vai direto para o servidor de destino. Ela vai para o servidor proxy, que então a encaminha para o destino. A resposta volta para o proxy e, em seguida, é enviada para você.

### Para que serve: 
- Pode ser usado para segurança (filtrando conteúdo), privacidade (escondendo seu IP real) ou para cache (acelerando o acesso a sites frequentemente visitados).

## Diferenças entre HTTP e HTTPS

* A principal diferença é a segurança. O HTTPS usa o protocolo SSL/TLS para criptografar a comunicação entre o cliente e o servidor.

### HTTP: 
- Dados trafegam em texto claro, sem criptografia. Inseguro para informações sensíveis.

### HTTPS: 
- Dados são criptografados, tornando-os ilegíveis para terceiros. Essencial para segurança e privacidade.

## Códigos HTTP e Verbos de Requisição

### Principais Categorias de Códigos HTTP

- São códigos de status que o servidor envia ao cliente na resposta, indicando o resultado da requisição.

### 2xx (Sucesso): 
- A requisição foi recebida, entendida e aceita com sucesso. Ex: 200 OK (requisição bem-sucedida).

### 4xx (Erro do Cliente): 
- O cliente cometeu um erro. Ex: 404 Not Found (o recurso solicitado não existe), 401 Unauthorized (não autorizado).

### 5xx (Erro do Servidor): 
- O servidor falhou ao processar uma requisição válida. Ex: 500 Internal Server Error (um erro genérico no servidor), 503 Service Unavailable (servidor temporariamente indisponível).

### Verbos de Requisição
- São métodos que indicam a ação que o cliente quer realizar no servidor.

### GET: 
- Solicita dados de um recurso específico.

### POST: 
- Envia dados para o servidor para criar um novo recurso.

### PUT: 
- Envia dados para atualizar um recurso existente.

### DELETE: 
- Remove um recurso específico.

## Principais Tags do HTML e Seletores do CSS

-	<h1> a <h6>: Títulos.

-	<p>: Parágrafo.

-	<a>: Link.

-	<img>: Imagem.

-	<div>: Divisão genérica, usado para agrupar elementos.

-	<span>: Usado para agrupar elementos em linha.

-	<ul>, <ol>, <li>: Listas não ordenadas e ordenadas.

-	<header>, <nav>, <main>, <footer>: Elementos semânticos que ajudam a estruturar a página.

### Seletores do CSS

-	Tipo/Elemento: Seleciona por tag, ex: p { color: blue; } (todos parágrafos).

-	Classe: Por atributo class, ex: .classe { font-size: 16px; }.

-	ID: Por atributo id único, ex: #id { background: red; }.

-	Atributo: Por atributos, ex: [href] { text-decoration: none; } ou [type="text"].

-	Pseudo-classe: Estados, ex: :hover (ao passar mouse), :first-child.

-	Combinadores: Relações, ex: div p (descendentes), div > p (filhos diretos), div + p (irmão adjacente), div ~ p (irmãos gerais)

-	Universal: * { margin: 0; } (todos elementos).

-	Agrupados: h1, h2 { color: green; 
 
### O que é uma webview
* Uma WebView é um componente de um aplicativo nativo (como um app para Android ou iOS) que permite exibir conteúdo da web dentro desse aplicativo. Em vez de abrir o navegador externo do seu celular, uma WebView renderiza uma página web diretamente dentro da interface do aplicativo.
### Para que serve: 
- É muito útil para mostrar conteúdo dinâmico que não precisa de uma interface nativa complexa, como páginas de "termos de uso", artigos de blog ou até mesmo parte de uma loja virtual, tudo sem sair do aplicativo.

###	Referencias:
[Git - Documentação]	
[Git - O que é Git?]
[Sobre o Git - GitHub Docs]
[Git - Documentação do git]
[Sobre o GitHub e o Git - GitHub Docs]
[GitHub – Wikipédia, a enciclopédia livre]
[ Aplicativos nativos vs aplicativos Webview - Qual é a melhor escolha para o seu negócio?]

(https://developer.mozilla.org/en-US/docs/Web/CSS/Type_selectors)

(https://www.w3schools.com/tags/ref_byfunc.asp)

(https://www.geeksforgeeks.org/html/html-tags-a-to-z-list/)

(https://www.juniper.net/documentation/us/en/software/junos/user-access/topics/concept/dns-proxy-overview.html)

(https://quizlet.com/study-guides/common-network-protocols-and-their-ports-a9209596-f9e4-40ba-9c8c-e07d6ca234a4)

(https://www.geeksforgeeks.org/computer-networks/protocols-application-layer/)

(https://dev.to/binoy123/comm-protocols-server-client-dynamics-54g2)
