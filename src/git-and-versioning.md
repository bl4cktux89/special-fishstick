# anotacoes realizadas durante o curso online da ada - bootcamp devops

## git

### aula 1

- software open source utilizado para realizar versionamento de código
- a cada commit, o git guarda e registra um snapshot para registrar um checkpoint do trabalho executado

> versionamento: registro de mudanças de arquivos

### aula 2

- baixar git (unix based systems) ou github desktop (windows e mac)

para verificar a versão instalada execute o comando

```bash
git --version
```

também é possível utilizar o git diretamente no vscode

### aula 3

> vamos utilizar o github como plataforma de repositórios remota

- para trazer um repositório para o computador
    - clique em code
    - copie o endereço https ou o ssh
    - abra o CMD ou terminal de sua preferência
    - execute o comando
    ```bash
    git clone <endereço https ou ssh>
    ```

### aula 4

estados do git:
- untracked (não rastreado)
- unmodified (não modificado)
- modified (modificado)
- staged (preparado)

para mostrar o status da branch atual e qual arquivo foi modificado, execute o comando:

```bash
git status
```

### aula 5

unmodified - já faz parte do ultimo commit -> modified - modificou algo -> git add para staged e no fim commit para voltar para unmodified.
git diff, para mostrar as linhas que foram modificadas

linhas vermelhas - removidas
linhas verdes - adicionadas

> sempre colocar mensagens claras no commit

### aula 6

inserir um único arquivo ao rastreio do git, digite o comando:
```bash
git add <nome-do-arquivo>
```

para adicionar todos os arquivos que estão na pasta atual:
```bash
git add .
```

para realizar o registro das mudanças efetuadas, digite o comando:
```bash
git commit -m "<mensagem a ser enviada no commit>"
```

para visualizar o histórico de commmits, bem como as hashs criadas para cada um deles, execute o comando:
```bash
git log 
```

> aprofundar mais o comando *git restore*
para descartar as alterações em arquivos específicos em seu repositório git:
```bash
git restore
```

### aula 7

#### fluxo de alteração de estados do git
adicionar para a área de preparo (staged):
```bash
git add
```
salvar o estado atual:
```bash
git commit
```
para enviar as alterações realizadas ao repositório remoto:
```bash
git push <verificar opções>
```
para trazer do repositório remoto e fazer um merge local:
```bash
git pull <verificar opções>
```

> *** CUIDADO AO USAR O GIT PULL ***

### aula 8

> fazer um overview do github

### aula 9

git branch testing
git log --oneline -decorate - para mostrar em qual branch o HEAD está
git checkout "testing" - para trocar o HEAD para outra branch
gitignore, para ignorar alguns arquivos
branch ajuda separar em fluxos

### aula 10

git branch, para mostrar qual branch está sendo acessada
git checkout master, para voltar o HEAD para master
git merge testing, unindo os fluxos das duas branch e retorna o fluxo principal para master


