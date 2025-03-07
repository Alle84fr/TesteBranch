Tem como fazer pull de forma mais rápida de todas as branchs? 
ou faz uma por uma
git pull origin main
git pull origin novobraco1
git pull origin novobraco2 ...

ou faz 
1° git fetch --all
2° git branch -r
3° git branch -r | grep -v '\->' | while read remote; do git branch --track "${remote#origin/}" "$remote"; done
4° git pull --all

sobre push all, está correto a forma de fazer?
git push --all origin
