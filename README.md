# Guia de Contribuição IT Girls - Garotas na Tecnologia da Informação

Esse é um guia de contribuição do IT GIRLS - Garotas na tecnologia da informação para desenvolvimento de software. Este guia possui o objetivo de orientar os membros do IT GIRLS que desejam desenvolver algum software durante o projeto, neste documento apresentaremos alguns conceitos de Git e Github, tutoriais de como se trabalhar com o Github e os padrões que devem ser seguidos durante o processo de desenvolvimento nesta organização.

*  Objetivos pelos quais está se fazendo este guia.
    
*   Descrição do conteúdo.
    
*  Índice

## Fluxo geral de trabalho

- **Criando um novo projeto**
<br/><br/>
**O que é um repositório?** <br/><br/>
Repositório é um diretório em que os arquivos dos seus projetos ficam armazenados.<br/><br/>
**Como criar um novo repositório** <br/><br/> 1. Abra o Github, faça login em sua conta e clique em New repository <br/><br/>

<p align="center">
    <img src="https://miro.medium.com/max/580/0*3AyGbHegYGjJgmKk." width="auto" height="250px" />
</p>

<br/><br/>2. Em seguida, coloque o nome e a descrição do repositório que você está criando e por fim clique em Create repository <br/><br/>

<p align="center">
    <img src="https://guides.github.com/activities/hello-world/create-new-repo.png" width="auto" height="300px" />
</p>

<br/><br/>3. Pronto, seu repositório foi criado. <br/><br/> **Clonando um projeto existente** <br/><br/> Ao criar um repositório no Github, este passa a existir como um repositório remote, o qual pode ser clonado, criando uma cópia local no seu computador e sincronizando entre esses dois ambientes (remote e local). <br/><br/> Clique no botão Clone or Download e, em seguida, clique no ícone "copiar para área" Agora abra um terminal e execute o seguinte comando git: <br/><br/>`git clone “url que você acabou de copiar”`  <br/><br/> em que “url que você acabou de copiar” (sem aspas) é a URL do repositório.<br/>
![Imagem](https://docs.github.com/assets/images/help/repository/remotes-url.png) <br/><br/>
- **Fork** <br/><br/> **O que é um fork?** <br/><br/>Fork é uma cópia que você faz de um repositório já existente. A cópia feita será destinada ao perfil de quem está fazendo o fork.<br/><br/> **Como criar um fork** <br/><br/> 1. Abra no repositório que você deseja “forkar”<br/>2. Clique no botão em destaque na imagem. <br/><br/>![Imagem](https://blog.da2k.com.br/uploads/2015/02/fork-repository.png)<br/><br/> 3. Selecione o perfil de destino do fork (caso apareça para você selecionar).<br/><br/>
-   **Commits** <br/><br/>**O que é um commit?**<br/><br/>Commits são registros da última versão de nosso código. Estes vão carregar tudo que foi alterado em nosso projeto para que, quando precisarmos, possamos voltar ao commit em que possuíamos a versão que gostaríamos de utilizar. <br/><br/> **Como fazer um commit** <br/><br/>Primeiro devemos configurar qual o repositório remoto. Execute o seguinte comando utilizando a url de seu repositório:<br/><br/>`git remote add origin "url do seu repositório`<br/><br/>Dessa forma, você configurou o remote origin para o Github. Você já pode subir seus commits para o Github usando o git push, mas na primeira vez o comando deve ser executado para configurar a branch master para o github. Assim, em sua primeira execução o comando realizado deve ser:<br/><br/>`git push -u origin master`<br/><br/>Nas próximas execuções, execute o seguinte comando:<br/><br/>`git push origin`<adicione-o-nome-de-sua-nova-branch><br/><br/>Com esse comando você irá subir seus commits para o Github. Ao executar este comando será solicitado o usuário e senha para autenticar no Github. Para adicionar as alterações que você realizou, execute o segundo comando:<br/><br/>`git add .`<br/><br/>Para visualizar as mudanças que você realizou, bem como todo estado de seu projeto, execute:<br/><br/>`git status`<br/><br/>Para confirmar as alterações realizadas, use o comando:<br/><br/>`git commit -m “comentários das alterações”`<br/><br/> **Padrão de commit**<br/><br/>Os padrões de commits desta organização deverão seguir a seguinte estrutura:<br/><br/><Label> `<descrição> (<Nº id da issue>)`<br/><br/>Todos os commits nos projetos desta organização deverá seguir as seguintes exigências:<br/><br/> 1 - Estar em português;<brq><br/> 2 - Estar coerente e coeso;<br/> 3 - Um commit por funcionalidade, etapas da criação da funcionalidade ou arquivo/biblioteca/dependência adicionado/removido.<br/> 4 - A descrição deve ser breve.. <br/><br/>
- **Branch**<br><br/>**O que é uma branch?**<br/><br/>Branch é uma maneira de organizar nosso trabalho com versionamento de código. Nós possuímos uma branch chamada master e nesta temos a versão oficial do nosso projeto. Quando vamos fazer uma alteração, podemos criar uma ramificação da master e trabalhar somente nela, sem afetar o código oficial. Ao finalizarmos nosso trabalho na nossa ramificação, então podemos fazer a junção com a master.<br/><br/> **Como criar uma branch**<br/><br/>Mude para o diretório no seu computador (caso você ainda não esteja lá) utilizando o comando:<br>
`cd “seu diretorio”`<br/><br/>Para criar uma ramificação, execute o seguinte comando:<br/><br/>`git checkout -b` <adicione-o-nome-de-sua-nova-branch><br/><br/> **Padrão de branch**<br/><br/>O padrão do nome de branch utilizado nessa organização deverá obedecer o seguinte padrão:<br/><br/><Label>`/<Nº id da issue>`<br/><br/>
- **Issues**<br/><br/> **O que é uma Issue?**<br/><br/>Uma issue é uma representação de uma tarefa. Com isso ela tem um ciclo de vida, possui seus tipos e a pessoa responsável por resolvê la.<br/><br/> **Como criar uma issue?**<br/><br/>**{}**<br/>**Labels**<br/> **O que é um Label?**<br/> **Padrões de Labels** <br/><br/>
- **Pull Request**<br/><br/> **O que é um Pull Request?**<br/><br/>Efetuar um Pull Request significa informar que você irá implementar as mudanças criadas na sua branch ao repositório master. Os colaboradores do repositório podem aceitar ou negar a Pull Request. Ao abrir um Pull Request você pode revisar e discutir seu trabalho com os colaboradores.<br/><br/> **Como submeter um Pull Request?**<br/><br/>Acesse a conta do repositório original no Github, e então você verá um botão Compare & pull request. Clique nesse botão. <br/><br/>![Imagem](https://blog.da2k.com.br/uploads/2015/02/message-pull-request.png)<br/><br/>Nesse momento, você será direcionado para a tela em que irá criar o pull request, podendo conferir se as alterações que aparecem realmente correspondem às suas modificações que você fez:<br/><br/> 1. O base fork é o diretório padrão. <br/> 2.  Ao lado, a branch para a qual vou enviar meu pull request. <br/> 3. A head fork é o seu repositório, que você forkou. <br/> 4. E por fim, em compare a branch que você alterou<br/><br/>
Depois disso, você deve colocar um título no seu pull request, para que, ao visualizar a listagem de pull requests, fique fácil saber do que se trata. Lembre-se de comentar porque você está fazendo esse pull request, e porque esse ajuste que você fez, faz sentido para o repositório.<br/>
Confira as informações, e clique em create pull request.<br/><br/>
- *Review*<br/>
- *Revisando o código*<br/><br/>**Como criar um manual do sistema?**<br/><br/>**Licenças**
