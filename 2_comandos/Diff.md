# Diff

De volta ao caso no qual um time de desenvolvedores resolveu um erro em um determinado projeto e agora você quer analisar quais foram as atitudes tomadas por eles.
De modo a analisar o que foi alterado nos arquivos, utilizaremos o comando **git diff nomedoarquivo.extensaodoarquivo**

Esse comando retornará a parte do código que foi alterada acomapanhada de alguns símbolos, são eles:

- O sinal "+", indicando o que foi **adicionado**
- O sinal "-", indicando o que foi **removido**

Cuidado!<br>
Não utilize o comando **git diff** após o comando **git add** em um mesmo arquivo. Não será possível visualizar as alterações pois as mesmas já estão no Index, prontas para sofrerem o commit.