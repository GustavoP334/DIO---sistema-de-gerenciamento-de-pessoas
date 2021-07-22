<h2>Digital Innovation: Expert class - Desenvolvendo um sistema de gerenciamento de pessoas em API REST com Spring Boot</h2>
<p>Nesta live coding vamos desenvolver um pequeno sistema para o gerenciamento de pessoas de uma empresa através de uma API REST, criada com o Spring Boot.</p>

<p>Durante a sessão, serão desenvolvidos e abordados os seguintes tópicos:</p>
<ul>
<li>Setup inicial de projeto com o Spring Boot Initialzr</li>
<li>Criação de modelo de dados para o mapeamento de entidades em bancos de dados</li>
<li>Desenvolvimento de operações de gerenciamento de usuários (Cadastro, leitura, atualização e remoção de pessoas de um sistema).</li>
<li>Relação de cada uma das operações acima com o padrão arquitetural REST, e a explicação de cada um dos conceitos REST envolvidos durante o desenvolvimento do projeto.</li>
<li>Desenvolvimento de testes unitários para validação das funcionalidades</li>
<li>Implantação do sistema na nuvem através do Heroku</li>
</ul>
<p>Para executar o projeto no terminal, digite o seguinte comando:</p>

<div class="highlight highlight-source-shell position-relative"><pre>mvn spring-boot:run </pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="mvn spring-boot:run 
" tabindex="0" role="button">
      <svg aria-hidden="true" viewBox="0 0 16 16" version="1.1" data-view-component="true" height="16" width="16" class="octicon octicon-clippy js-clipboard-clippy-icon m-2">
    <path fill-rule="evenodd" d="M5.75 1a.75.75 0 00-.75.75v3c0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75v-3a.75.75 0 00-.75-.75h-4.5zm.75 3V2.5h3V4h-3zm-2.874-.467a.75.75 0 00-.752-1.298A1.75 1.75 0 002 3.75v9.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 13.25v-9.5a1.75 1.75 0 00-.874-1.515.75.75 0 10-.752 1.298.25.25 0 01.126.217v9.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-9.5a.25.25 0 01.126-.217z"></path>
</svg>
      <svg aria-hidden="true" viewBox="0 0 16 16" version="1.1" data-view-component="true" height="16" width="16" class="octicon octicon-check js-clipboard-check-icon color-text-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<p>Após executar o comando acima, basta apenas abrir o seguinte endereço e visualizar a execução do projeto:</p>

<div class="snippet-clipboard-content position-relative"><pre><code>http://localhost:8080/api/v1/people
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="http://localhost:8080/api/v1/people
" tabindex="0" role="button">
      <svg aria-hidden="true" viewBox="0 0 16 16" version="1.1" data-view-component="true" height="16" width="16" class="octicon octicon-clippy js-clipboard-clippy-icon m-2">
    <path fill-rule="evenodd" d="M5.75 1a.75.75 0 00-.75.75v3c0 .414.336.75.75.75h4.5a.75.75 0 00.75-.75v-3a.75.75 0 00-.75-.75h-4.5zm.75 3V2.5h3V4h-3zm-2.874-.467a.75.75 0 00-.752-1.298A1.75 1.75 0 002 3.75v9.5c0 .966.784 1.75 1.75 1.75h8.5A1.75 1.75 0 0014 13.25v-9.5a1.75 1.75 0 00-.874-1.515.75.75 0 10-.752 1.298.25.25 0 01.126.217v9.5a.25.25 0 01-.25.25h-8.5a.25.25 0 01-.25-.25v-9.5a.25.25 0 01.126-.217z"></path>
</svg>
      <svg aria-hidden="true" viewBox="0 0 16 16" version="1.1" data-view-component="true" height="16" width="16" class="octicon octicon-check js-clipboard-check-icon color-text-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div></div>

<p>São necessários os seguintes pré-requisitos para a execução do projeto desenvolvido durante a aula:</p>

<ul>
<li>Java 11 ou versões superiores.</li>
<li>Maven 3.6.3 ou versões superiores.</li>
<li>Intellj IDEA Community Edition ou sua IDE favorita.</li>
<li>Controle de versão GIT instalado na sua máquina.</li>
<li>Conta no GitHub para o armazenamento do seu projeto na nuvem.</li>
<li>Conta no Heroku para o deploy do projeto na nuvem</li>
</ul>

<p>Abaixo, seguem links sobre tópicos mencionados durante a aula:</p>

<ul>
<li><a href="https://sdkman.io/" rel="nofollow">SDKMan! para gerenciamento e instalação do Java e Maven</a></li>
<li><a href="https://www.jetbrains.com/idea/download" rel="nofollow">Referência do Intellij IDEA Community, para download</a></li>
<li><a href="https://resources.jetbrains.com/storage/products/intellij-idea/docs/IntelliJIDEA_ReferenceCard.pdf" rel="nofollow">Palheta de atalhos de comandos do Intellij</a></li>
<li><a href="https://spring.io/" rel="nofollow">Site oficial do Spring</a></li>
<li><a href="https://start.spring.io/" rel="nofollow">Site oficial do Spring Initialzr, para setup do projeto</a></li>
<li><a href="https://www.heroku.com/" rel="nofollow">Site oficial do Heroku</a></li>
<li><a href="https://git-scm.com/" rel="nofollow">Site oficial do GIT</a></li>
<li><a href="http://github.com/">Site oficial do GitHub</a></li>
<li><a href="https://projectlombok.org/" rel="nofollow">Documentação oficial do Lombok</a></li>
<li><a href="https://mapstruct.org/" rel="nofollow">Documentação oficial do Map Struct</a></li>
<li><a href="https://restfulapi.net/" rel="nofollow">Referência para o padrão arquitetural REST</a></li>
</ul>

<p><a href="https://drive.google.com/file/d/1crVPOVl6ok2HeYjh3fjQuGQn2lDZVHrn/view?usp=sharing" rel="nofollow">Neste link</a>, seguem os slides apresentados como o roteiro utilizado para o desenvolvimento do projeto da nossa sessão.</p>**