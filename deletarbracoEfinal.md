sem querer criei uma branch chamada primeirobraco, vou deletar

git branch -v
  origin/bracoFinal
  origin/main
  origin/novoBraco
  origin/primeiroBraco

1° git branch -d primeirobraco

dei git branch -r e continuou aparecendo o branch então

1° git push origin --delete primeiroBraco
aqui amanda repositório remoto deletar a branch

2° git fetch --primeiroBraco
é boa prática sempre atualizar a lista de branch

para verificar
git branch -r
  origin/bracoFinal
  origin/main
  origin/novoBraco
  SAIU A BRANCH PRIMEIORBRACO

  SEMPRE LEMBRAR DE ADD E COMMIT