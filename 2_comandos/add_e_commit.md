## Add e Commit

No mundo da programação, comumente ocorrem situações nas quais com o passar do tempo trabalhando em determinado projeto, começamos a esquecer o motivo de ter feito algum passo anterior ou que área do código necessita de atenção no momento. Com os comandos a seguir, aprenderemos a editar e salvar nossos arquivos quantas vezes quisermos e, quando tudo estiver pronto, salvaremos nossas alterações que futuramente serão enviadas ao nosso repositório.

# Add

O comando 
```
git add "arquivo"
```

Adicionará quaisquer arquivos em um lugar chamada Index, citado anteriormente. Ao executar este comando não estamos adicionando um arquivo novo ao repositório em questão, mas sim informando que o arquivo (novo ou não) está sendo preparado para entrar na próxima revisão do repositório.<br>

Dica: Caso queira adicionar mais de um arquivo ao Index, basta entrar com o comando "git add ." que todos os arquivos de um dado diretório serão adicionados.

# Commit

O commit pode ser comparado aos registros em um diário, ao executar o comando abaixo:
```
git commit -m "comentário"
```

será realizado o procedimento de commit, que consiste em acessar os arquivos no Index e criar uma revisão com um número e um comentário que poderá ser visualizado por todos os colaboradores do projeto.


## Exemplo

Veja abaixo um exemplo básico de utilização de git e commit, seguidos estes passos:


- Crie um arquivo chamado 42.txt na pasta raiz de seu repositório e adicione algum conteúdo a ele
- Adicione o arquivo criado a lista de futuras alterações com o comando git add <arquivo>
- Crie um registro **commit** informando na mensagem uma descrição da sua ação

```
echo "Houston, We have a problem!" > 42.txt
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

Portanto, um commit nada mais é do que  adição/edição/remoção de um ou mais arquivos de um determinado repositório.




