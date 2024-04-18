

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


