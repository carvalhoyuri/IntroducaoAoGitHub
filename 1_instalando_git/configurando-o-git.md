#Configurando o Git
Para obter um acesso mais simplificado ao Git, são necessários alguns passos. Durante esta tarefa, determinaremos que sempre que necessário, serão fornecidos e-mail e senha ao GitHub, sem necessida de digitar toda vez que o acesso for requerido.<br>

Para abrir um terminal Git no Windows, crie uma pasta no local de preferência, dê um clique com o botão direito do mouse e escolha a opção **Git Bash Here**.
Em sistemas Linux/Mac, o Git estará disponível através do próprio console.<br>

Então, com o terminal aberto, digite os seguintes comandos:

```

git config --global user.name "SEU NOME"
git config --global user.email "SEU E-MAIL"

```


As configurações inseridas ficarão guardadas no arquivo **~/.gitconfig**, sendo ~ o seui diretório home.
No Windows, por exemplo, encontramos esse diretório em: **c:\Usuarios\username\.gitconfig**. 
