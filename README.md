# Estrutura Básica de Um Commit
![image](https://github.com/SarahSHortiz/committeste/assets/112779900/8aa63fcf-6cdb-4e1f-b9e8-dffa4a4dd0fb)

```feat```- Commits do tipo feat indicam que seu trecho de código está incluindo um novo recurso (se relaciona com o MINOR do versionamento semântico).

```fix``` - Commits do tipo fix indicam que seu trecho de código commitado está solucionando um problema (bug fix), (se relaciona com o PATCH do versionamento semântico).

```docs``` - Commits do tipo docs indicam que houveram mudanças na documentação, como por exemplo no Readme do seu repositório. (Não inclui alterações em código).

```test``` - Commits do tipo test são utilizados quando são realizadas alterações em testes, seja criando, alterando ou excluindo testes unitários. (Não inclui alterações em código)

```build``` - Commits do tipo build são utilizados quando são realizadas modificações em arquivos de build e dependências.

```perf``` - Commits do tipo perf servem para identificar quaisquer alterações de código que estejam relacionadas a performance.

```style``` - Commits do tipo style indicam que houveram alterações referentes a formatações de código, semicolons, trailing spaces, lint... (Não inclui alterações em código).

```refactor``` - Commits do tipo refactor referem-se a mudanças devido a refatorações que não alterem sua funcionalidade, como por exemplo, uma alteração no formato como é processada determinada parte da tela, mas que manteve a mesma funcionalidade, ou melhorias de performance devido a um code review.

```chore``` - Commits do tipo chore indicam atualizações de tarefas de build, configurações de administrador, pacotes... como por exemplo adicionar um pacote no gitignore. (Não inclui alterações em código)

```ci``` - Commits do tipo ci indicam mudanças relacionadas a integração contínua (continuous integration).

```raw``` - Commits to tipo raw indicam mudanças relacionadas a arquivos de configurações, dados, features, parametros.

```cleanup``` - Commits do tipo cleanup são utilizados para remover código comentado, trechos desnecessários ou qualquer outra forma de limpeza do código-fonte, visando aprimorar sua legibilidade e manutenibilidade.

```remove``` - Commits do tipo remove indicam a exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas, reduzindo o tamanho e a complexidade do projeto e mantendo-o mais organizado.

# Como Iniciar Um Commit
```
git add .
```
```
git cz
```
(escolher as configs)

![image](https://github.com/SarahSHortiz/committeste/assets/112779900/77e96fb5-f7ea-41fe-8bc4-527ad80b1878)
```
git push
```
(para enviar ao repositório remoto)

# Enviar Commits
```
git push
```
# Puxar Informações e Atualizações de Repositórios Onlines/Remotos
```
git pull
```


## Etrutura do commitlint.config.js 
![image](https://github.com/SarahSHortiz/committeste/assets/112779900/3ce75e96-6756-49cf-807b-88056aeda201)

## Estrutura do package.json 

![image](https://github.com/SarahSHortiz/committeste/assets/112779900/890a1742-4e31-43c0-8849-cdfbdb719ef2)

É necessário installar o Commitlint e Husky juntamente com o Commitizen

```json
{
  "name": "lintcommit",
  "version": "1.0.0",
  "main": "teste.py",
  "license": "MIT",
  "scripts": {
    "commit": "git-cz",
    "test": "echo 'No tests specified'"
  },
  "husky": {
    "hooks": {
      "commit-msg": "commitlint -E HUSKY_GIT_PARAMS"
    }
  },
  "config": {
    "commitizen": {
      "path": "cz-conventional-changelog"
    }
  },
  "devDependencies": {
    "@commitlint/cli": "^19.2.2",
    "@commitlint/config-conventional": "^19.2.2",
    "cz-conventional-changelog": "^3.3.0",
    "husky": "^9.0.11"
  }
}
```
# Commitlint
```
npm install  @commitlint/config-conventional @commitlint/cli -D
```
```
npm install --save-dev @commitlint/config-conventional @commitlint/cli
```
```
echo .commitlintrc
```
# Husky
```
npm i husky
```
```
npm install --save-dev husky
```
```
git commit -m "Keep calm and commit"
```
```
npx husky init
```
# Commitizen
```                                                                                        
npm install -g commitizen
```
```                                                                                      
npx cz
```
```
npm install commitizen -g
```
```                                                                                     
commitizen init cz-conventional-changelog --save-dev --save-exact
```
```
git commit                                                                                                         
```
(caso não dê certo e conste erro)
```
npm run commit -- --retry
```
```
git cz
```
## Caso o User Não Esteja Logado
```
git config --global user.email "seu email "
```
```
 git config --global user.name "seu nome de user"                 

```


