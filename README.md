# DIO | Repositorio para armazenar resumos sobre Git e Githuub!

Obs -> win + '.' : abre a aba de emojis!  

## 📚 Documentacao
- [Documentacao do Git](https://git-scm.com/)
- [Documentacao do GitHub](https://docs.github.com/pt)

## Resumos das aulas

### ✨ iniciando um repositorio
```
git init
```
```
git clone <url_repositorio>
```
### clonando com uma branch especifica de um repositorio remoto
```
git clone <url_repositorio> --branch <nome_branch> --single-branch
```
### 🔗 'linkando' com um repositorio remoto
```
git remote add origin <url_repositorio>
```
### ➕ adicionando arquivos a um repositorio local
```
git add <nome_arquivo>
```
❗ adcionando todo a pasta onde o .git esta contido
```
git add .
```
### ✔ commitando o projeto; inserindo uma mensagem
```
git commit -m "feat: estudando git"
```
### 📌enviando os arquivos add ao repositorio remoto
- -u = --set-upstream
```
git push -u origin main
```
### 💕 busca as alteracoes no repositorio remoto
```
git pull
```
### buscando historico dos commits
```
git log
```
### busncando alteracoes desconhecidas pelo git
```
git status
```
## 🔃 Desfazendo alteracoes no repositorio local

### restaurando um arquivo modificado
```
git restore <nome_arquivo>
```
### 🗃 alterando a menssagem do ultimo commit
```
git commit --amend -m "mensagem" 
```
### 💢 desfazendo um ultimo commit

--> o hash do commit pode ser localizado no git log
--> --soft: add os arquivos na area de preparacao e desfaz o commit
--> --mixed: e padrao, remove os arquivos da area de preparacao
--> --hard:  limpa a arvore das alteracoes anteriores junto com o commit
```
git reset (--soft, --mised, --hard) <hash_commit>
```

### retirando os arquivos da area de preparacao
```
git restore  --staged <arquivo>
```
ou...
```
git reset <arquivo>
```
### Trabalhando com Branchs
- e uma ramificacao do projeto
- main e a principal
- git branch -M main : renomeia a branch "master" para "main"
- git branch -m master main : equivale ao comando acima
  
## 💛 criando uma branch
```
git checkout -b <nome_branch>
```
## 💞 mudando de branch
```
git checkout <nome_branch>
```
## 💕 mesclando branch atual com outra branch
```
git merge <nome_outra_branch>
```
## 💥 deletando branch
```
git branch -d <nome_branch>
```

## verificando em que branch o projeto se encontra
```
git branch
```
## litando as branchs do projeto
```
git branch -v
```

- git pull = git fetch + git merge

## Comandos uteis


