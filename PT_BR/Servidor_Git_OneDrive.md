
<p align="center">
<img src="https://git-scm.com/images/logos/downloads/Git-Logo-1788C.png" alt="git" style="width:210px;"/> <img src="https://www.logo.wine/a/logo/OneDrive/OneDrive-Logo.wine.svg" alt="OneDrive" style="width:200px;"/>
</p>
<h1 align="center">Criando um servidor Git no OneDrive</h1>
<h3 align="center">Também funciona com Google Drive, Dropbox etc..</h3>
<br>
<p>Inicialize o servidor git dentro da pasta compartilhada no OneDrive com o parâmetro --bare, ele fará com que você não inicialize um simples repositório local mas sim um repositório "pushable", que fará o armazenamento do código fonte.</p>


    OneDrive_$ git init --bare

<p>Agora clone o repósitorio passando o caminho do repositório criado no OneDrive, ele precisa começar com o caminho "file:///". Utilize aspas duplas caso o nome da pasta tenha espaços.</p>

    git clone file:///"C:\Users\gabriel.gontijo\OneDrive\repo"

<p>Caso o repositório seja compartilhado por mais de uma pessoa, você pode ter algum problema por conta da sincronização destas soluções. Evite criar múltiplos commits ao mesmo tempo.</p>