vendo se corrijo o push --all

1° git remote -v

deve aparecer algo assim
origin  https://github.com/seu-usuario/seu-repositorio.git (fetch)
origin  https://github.com/seu-usuario/seu-repositorio.git (push)

2° git config --global credential.helper store
aqui, pelo que entendi o git arruma credenciais incorretas e desatualizadas
pode ser que peça nome de usuário, senha ou token

lembrar de dar git add . e commit

3° git push --all origin

foi