## Add e Commit

No mundo da programação, comumente ocorrem situações nas quais com o passar do tempo trabalhando em determinado projeto, começamos a esquecer o motivo de ter feito algum passo anterior ou que área do código necessita de atenção no momento. Com os comandos a seguir, aprenderemos a editar e salvar nossos arquivos quantas vezes quisermos e, quando tudo estiver pronto, salvaremos nossas alterações que futuramente serão enviadas ao nosso repositório.

# Add

O comando 
```
git add "arquivo"
```

Realizará a ação de adicionar o referido arquivo que se encontra no diretório do seu sistema à uma área temporária chamada Index, essa operação faz parte do fluxo de trabalho no Git.<br>
Podemos imaginar esta etapa de adição de arquivos ao Index, como pequenos checkpoints em nosso código, como quando necessitamos adicionar e testar novas funcionalidades ou fazer alguma alteração da qual não temos certeza se irá funcionar ou não. Sendo assim, é possível realizar testes ao passo em que construímos o código e salvar somente sua versão final com o comando commit que veremos posteriormente.<br>

Veja um esquema de funcionamento do comando add:

![gitadd](/images/gitadd.png)

Ao executar este comando, estamos informando ao git que o arquivo referenciado possivelmente entrará na próxima autalização do projeto.<br>

Dica: Caso queira adicionar mais de um arquivo ao Index ao mesmo tempo, basta entrar com o comando "git add ." que todos os arquivos de um dado diretório serão adicionados.

# Commit

O commit pode ser comparado aos registros em um diário, ao executar o comando abaixo:
```
git commit -m "comentário"
```

será realizado o procedimento de commit, no qual o Git acessará a área do Index, buscará os arquivos ali presentes e criará uma revisão com um número e um comentário que poderá ser visualizado por todos os colaboradores do projeto.<br>
Podemos compara o comando **git add** com a demarcação de um terreno, podemos muitas vezes mudar a forma deste terreno enquanto pensamos na melhor maneira de construir, e o comando **git commit** é a construção dos muros do terreno em si, na qual será explicitada o porquê demarcamos o terreno daquele jeito ou ainda, o porquê alteramos determinada parte do mesmo.
Perceba que é muito mais fácil realizar alterações na demarcação do terreno tendo uma visão virtual (Index) de sua construção do que construir os muros e então destruir, e então construir novamente.<br>

Veja um esquema do processo de commit abaixo:

![commithead](/images/head.png)




## Exemplo

Veja abaixo um exemplo básico de utilização de git e commit, seguidos estes passos:


- Crie um arquivo chamado 42.txt na pasta raiz de seu repositório e adicione algum conteúdo a ele
- Adicione o arquivo criado a lista de futuras alterações com o comando **git add arquivo**
- Crie um registro **commit** informando na mensagem uma descrição da sua ação

```
echo "Houston, We have a problem!" > 42.txt //Este comando criará um arquivo chamado 42.txt e seu conteúdo será o argumento entre aspas logo após o comando echo. 
git add 42.txt
git commit -m "Criação de arquivo txt"
```

Suponhamos agora, que você cometeu um erro ao subir este arquivo no seu projeto, restando duas opções: reverter a ação ou sobrescrever. 
De modo a manter nossos registros anteriores e assim criar uma linha do tempo mais completa, iremos sobrescrever, seguindo estes passos:

- Altere o texto do arquivo 42.txt para "Don't Panic!"
- Salve o arquivo e adicione a lista de alterações novamente
- Crie um novo commit com a descrição da alteraçao feita

```
echo "Don't Panic!" > 42.txt
git add 42.txt
git commit -m "Alteração no texto do arquivo txt"
```

Portanto, um commit nada mais é do que  adição/edição/remoção de um ou mais arquivos em um determinado repositório.




