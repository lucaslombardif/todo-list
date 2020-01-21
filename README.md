# Todo app criado com ReactJS, Redux, e Firebase 
Um simples Todo com a capacidade de **excluir** e **desfazer a exclusão** cirado com  [Create React App](https://github.com/facebookincubator/create-react-app), [React Redux](https://github.com/reactjs/react-redux), e [Firebase](https://firebase.google.com/).

Teste a aplicação online em https://lucaslombardif.tech

## Tecnologias Utilizadas

- Create React App
- React Redux
- React Router
- React Router Redux
- Redux Thunk
- Redux Devtools Extension for Chrome
- Firebase SDK with OAuth authentication
- Immutable
- Reselect
- SASS


Como utilizar
-----------

```shell
$ git clone https://github.com/r-park/todo-react-redux.git
$ cd todo-react-redux
$ npm install
$ npm start
```

## Fazendo Deploy no Firebase 
#### Pré-requisitos:
- Crie uma conta grátis em https://firebase.google.com
- Crie um projeto em seu [Console da Conta Firebase](https://console.firebase.google.com)
- Configure os provedores de autenticação 

#### Configure esse app com os detalhes especifícos do seu projeto Firebase :
```json
// .firebaserc

{
  "projects": {
    "default": "your-project-id"
  }
}
```

```javascript
// src/firebase/config.js

export const firebaseConfig = {
  apiKey: 'your api key',
  authDomain: 'your-project-id.firebaseapp.com',
  databaseURL: 'https://your-project-id.firebaseio.com',
  storageBucket: 'your-project-id.appspot.com'
};
```

#### Instale a CLI do Firebase :
```shell
$ npm install -g firebase-tools
```

#### Faça o build e o Deploy:
```shell
$ npm run build
$ firebase login
$ firebase use default
$ firebase deploy
```


## Comandos NPM

|Comando|Descrição|
|---|---|
|`npm start`|Inicia o servidor de desenvolvimento @ `localhost:3000`|
|`npm run build`|Construa a aplicação gerando os arquivos estáticos no diretório`./build`|
|`npm test`|Teste sua aplicação|

### Credits by: https://github.com/r-park 


