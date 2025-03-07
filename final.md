deu muitos erros vamos lá
para dar pull de todas as branch

1° git fetch --all
atualiza a lista de branchs remotas/nuvem no local

aapareceu isso
remote: Enumerating objects: 9, done.
remote: Counting objects: 100% (9/9), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (6/6), 2.50 KiB | 183.00 KiB/s, done.
From https://github.com/Alle84fr/TesteBranch
 * [new branch]      bracoFinal -> origin/bracoFinal
   07fb335..70ac371  novoBraco  -> origin/novoBraco

lembrando que eu só tinha os branchs main e novoBraco feitos no meu computador/local

2° git branch -r

vê as branchs remotas

apareceu em vermelho
  origin/bracoFinal
  origin/main
  origin/novoBraco

3° git branch -r | grep -v '\->' | while read remote; do git branch --track "${remote#origin/}" "$remote"; done

criando uma branch local correspondente a remota
git branch -r -> lista todas branchs remotas
grep -v '\->' ->filtra branch inválida
git branch --track -> cada branch remota cria uma branch local correspondente e configura op tracking

4° atualiza/pull/download

git pull --all

5° entra na branch desejada git checkout bracoFinal ou a que deseja

eu dei git branch para ver se estou na branch certa

TENHO QUE VER SE É ASSIM MESMO COM O PROFESSOR