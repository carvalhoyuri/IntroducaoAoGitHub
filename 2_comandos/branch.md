# Branch

Já imaginou como seria interessante se em nossas vidas pudéssemos tomar uma decisão, ver os resultados e consequências e ainda tivéssemos a oportunidade de voltar atrás ou não?<br>
Pois bem, uma branch é justamente isso, um espécie de uma realidade alternativa ou universo paralelo que, em algum momento, irá se juntar com a realidade principal.<br>

Lembra do repositório que nós criamos? Ele nada mais é do que uma branch, é a nossa realidade principal, por isso, ele é denominado de Branch Master!<br>

Um comum cenário que um grupo encontra ao trabalhar em um mesmo código é a necessidade da resolução de um erro, e para tal, não há uma solução única, de modo que diferentes desenvolvedores podem tentar diferentes soluções.
E para não bagunçar tudo, eles criam uma branch, ramos do projeto principal, que são uma cópia exata dos mesmos. Ficando livres então para realizar alterações no código sem prejudicar o código principal.<br>

Veja então um exemplo no qual iremos adicionar um novo arquivo de texto porém não no diretório principal e sim, criando uma nova branch para isso.
A criação de uma nova branch é feita através do comando **git checkout -b <nome da branch>**
O comando **git branch** é útil para visualizar em qual branch você está em um determinado momento, apresentando um * na branch atual.

```
git checkout -b MundoParalelo
git branch
    master
*   MundoParalelo

echo "I'm your father!" > LukeDontOpen.txt
git add .
git commit -m "Inserção de novo arquivo"
```

Confira um esquema de todas as alterações feitas até aqui:

![branches](/images/branches.png)


