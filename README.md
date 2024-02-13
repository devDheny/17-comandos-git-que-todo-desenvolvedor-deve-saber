
# 17 comandos Git que todo desenvolvedor deve saber

Neste artigo, compartilharei e explicarei os 17 comandos do Git que todo desenvolvedor deveria saber.


## Gerenciando repositórios:

#### 1. `git init`: Este comando transforma um diretório em um repositório Git. É o primeiro passo para começar a usar o Git em um projeto.
```
git init my-project
```

#### 2. `git clone`: Este comando baixa um repositório remoto para o seu computador. É útil para começar a trabalhar em um projeto que já está hospedado em um serviço como o GitHub.
```
git clone https://github.com/user/project.git
```

#### 3. `git remote add`: Este comando conecta seu repositório local a um repositório remoto. Isso permite que você envie suas alterações para o repositório remoto e baixe as alterações de outros colaboradores.
```
git remote add origin https://github.com/user/project.git
```

#### 4. `git remote -v`: Este comando lista todos os repositórios remotos conectados ao seu projeto local. É útil para verificar se você está conectado ao repositório correto.
```
git remote -v
```

#### 5. `git fetch`: Este comando baixa as alterações do repositório remoto para o seu computador, mas não as mescla com suas alterações locais. É útil para manter seu repositório local atualizado com as últimas alterações do repositório remoto.
```
git fetch origin
```

#### 6. `git push`: Este comando envia suas alterações locais para o repositório remoto. É útil para compartilhar suas alterações com outros colaboradores ou para fazer backup do seu projeto.
```
git push origin master
```

#### 7. `git pull`: Este comando é um atalho para `git fetch` seguido de `git merge`. Ele baixa as alterações do repositório remoto e as mescla com suas alterações locais. É útil para atualizar seu repositório local com as últimas alterações do repositório remoto e mesclá-las com suas alterações locais
```
git pull origin master
```


## Trabalhando com branches

#### 8. `git branch`: Este comando cria uma nova branch. É útil para trabalhar em diferentes features ou correções de bugs sem afetar a branch principal do seu projeto.
```
git branch feature/new-feature
```

#### 9. `git checkout`: Este comando troca para uma branch específica. É útil para começar a trabalhar em uma branch diferente ou para verificar as alterações em uma branch diferente.
```
git checkout feature/new-feature
```

#### 10. `git branch -d`: Este comando exclui uma branch local. É útil para remover branches que você não precisa mais.
```
git branch -d feature/new-feature
```

#### 11. `git merge`: Este comando mescla uma branch com a branch atual. É útil para integrar as alterações de diferentes branches em uma única branch.
```
git checkout master
git merge feature/new-feature
```


## Gerenciando Alterações:

#### 12. `git status`: Este comando mostra o status das alterações no seu projeto. É útil para verificar quais arquivos foram modificados, quais arquivos estão no staging area e quais commits foram feitos.
```
git status
```

#### 13. `git add`: Este comando adiciona arquivos ao staging area para serem comitados. O staging area é uma área intermediária onde você pode preparar os arquivos para serem comitados.
```
git add index.html
```

#### 14. `git commit`: Este comando salva as alterações no staging area como um commit. Um commit é um registro permanente das alterações feitas no seu projeto.
```
git commit -m "Added new feature"
```

#### 15. `git reset`: Este comando desfaz as alterações feitas nos arquivos ou commits. É útil para corrigir erros ou para voltar para uma versão anterior do seu projeto.
```
git reset HEAD~1
```

#### 16. `git log`: Este comando mostra o histórico de commits do seu projeto. É útil para ver quais alterações foram feitas no projeto ao longo do tempo.
```
git log
```

#### 17. `git diff`: Este comando mostra as diferenças entre as versões dos arquivos. É útil para ver quais alterações foram feitas em um arquivo específico.
```
git diff index.html
```


#### Dicas Úteis:

-  Use aliases para os comandos que você usa com mais frequência.
- Use o `git help` para obter mais informações sobre qualquer comando.
- Pratique usando o Git em um projeto pessoal antes de usá-lo em um projeto profissional.


### Comandos bônus:
- `git stash`: Este comando salva as alterações não comitadas para que você possa trabalhar em outra coisa. É útil quando você precisa mudar de contexto e não quer perder as alterações que você já fez.
```
git stash
git checkout master
# Trabalhe na branch master
git checkout feature/new-feature
git stash pop
```
- `git rebase`: Este comando reorganiza a ordem dos commits na sua branch. É útil para deixar o histórico de commits mais limpo e organizado.
```
git checkout feature/new-feature
git rebase master
```
- `git bisect`: Este comando encontra o commit que introduziu um bug. É útil para depurar problemas e encontrar a causa de um bug.
```
git bisect start HEAD master
# Execute testes para identificar o commit com o bug
git bisect bad
git bisect good
# Continue repetindo os comandos `git bisect bad` e `git bisect good` até encontrar o commit com o bug
```

#### Observações:

- Os comandos bônus são mais avançados e podem ser mais difíceis de usar.
- É importante ter cuidado ao usar esses comandos, pois eles podem modificar o histórico de commits do seu projeto.
- É recomendável praticar o uso desses comandos em um projeto pessoal antes de usá-los em um projeto profissional.


*Com o conhecimento desses comandos básicos, você estará pronto para usar o Git para gerenciar seus projetos de desenvolvimento de software.*