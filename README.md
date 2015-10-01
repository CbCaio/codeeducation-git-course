### Primeira atividade - Realizando o primeiro commit:

1. [Aprender o b�sico sobre markdown](https://help.github.com/articles/markdown-basics)
2. Realizar o instru��es:
  1. touch arquivo.txt 
  2. vim git-commands.txt
  3. git add git-commands.txt
  4. git status
  5. vim README.md
  6. git add README.md
  7. git commit -m "Primeiro commit, arquivo contendo os comandos aprendidos do git"
  8. git push origin master

### Segunda atividade - Releases:
  1. git tag 0.1.0
  2. git push origin master --tags
  3. fazer novos commits e criar outra release

### Habilitar conex�o por ssh (git-bash):

Comando para gerar chave:
```
ssh-keygen -t rsa -b 4096 -C "email"
```

Ativando ssh-agent
```
eval `ssh-agent -s`
```

Adicionando chave ao ssh-agent:
```
ssh-add ~/.ssh/id_rsa
```

Testando conex�o com o github:
```
ssh -T git@github.com
```

Se tudo correr bem, agora apenas � necess�rio adiciona-la ao perfil do github, para copiar a chave para o clipboard:
```
clip < ~/.ssh/id_rsa.pub
```

>Importante: Lembrar de garantir que a conex�o com o reposit�rio remoto esteja sendo feita atrav�s do ssh
```
git remote set-url origin git@github.com:user/repository.git
```
