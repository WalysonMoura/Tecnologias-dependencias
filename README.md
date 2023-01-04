# 🛠️ Tecnologias/Ferramentas ultilizadas
* ### NPM  de instalação das tecnologias mais usadas por mim 

![mock1](https://user-images.githubusercontent.com/71772559/113493479-eceeda80-94b5-11eb-94ea-59e50e56a31f.png)

# Front-End <img src="https://github.com/rafaballerini/ReactHooks/blob/master/public/React.svg.png?raw=true" width="70px" >


* ## Instalação React / Next.JS / Styled-Components
```
yarn create next-app --nomeProjeto with-styled-components with-styled-components-app --typescript
```
```
yarn add next@13 
```
```
yarn add  next react react-dom    
```

* ## TypeScript  
```
yarn add typescript -D 
```
```
yarn add typescript @types/react @types/node -D 

```

* ## Style-components
```
 yarn add styled-components --save
```
```
 yarn add -D babel-plugin-styled-components
```

 Para utilizaçâo do Styled Components com Next é necessário a criação do arquivo `.babelrc` na raiz do projeto com as configurações a seguir:  


```.json
  {
  "presets": [
    "next/babel"
  ],
  "plugins": [
    [
      "styled-components",
      {
        "ssr": true,
        "displayName": true,
        "preprocess": false
      }
    ]
  ]
}
```

* ## React icons
[Buscar Icones](https://react-icons.github.io/react-icons/)
```
  yarn add react-icons --save 
```
* ## React Reveall
```
 yarn add react-awesome-reveal @emotion/react --save
```
* ## React Tilt [site](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--default)
```
yarn add react-parallax-tilt
```
* ## Animate.css
```
yarn add animate.css --save 
```
* ## Spline 3D
```
yarn add @splinetool/react-spline @splinetool/runtime
```

# Back-End 💻
* ## ambiente Node.js
```
 yarn init -y   
```
* ## Express
```
 yarn add express   
```
* ## TypeScript 
```
yarn add typescript @types/express @types/node -D 
```

* ## Configuração do TypeScript
```
yarn tsc --init 
```
```
yarn tsc
```

* ## compilar  TypeScript
```
yarn add ts-node-dev -D
```

* ## Type ORM

#### Com PostgreSQL 
```
 yarn add typeorm reflect-metadata pg
```

 ### Express-generator
```
yarn add express-generator -g
```
* ## Ejs
```
 express nomeProjeto --ejs   
```

* ## Sequelize
```
 yarn add sequelize
```
```
yarn add sequelize-cli -D
```
### Models co sequelize

```
yarn sequelize init:models
```

* ## MySQL 
```
yarn add install mysql2
```


* ## axios
```
 yarn add --save axios   
```

* ## GraphQL
```
 yarn add type-graphql graphql apollo-server class-validator reflect-metadata
 
```
```
 yarn add type-g
 
```

# CMS
* ## Prismic
```
 yarn add @prismicio/react @prismicio/client
```

# Ferramentas Extras

* [CSS Buttons](https://uiverse.io)
* [Neumorphism](https://neumorphism.io/#e0e0e0)
* [Efeito Vidro](https://css.glass/)
* [Box-Shadow CSS Generator](https://html-css-js.com/css/generator/box-shadow/)
* [FANCY-BORDER-RADIUS](https://9elements.github.io/fancy-border-radius/)

