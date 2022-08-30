# 🛠️ Tecnologias/Ferramentas ultilizadas
* ### NPM  de instalação das tecnologias mais usadas por mim 

![mock1](https://user-images.githubusercontent.com/71772559/113493479-eceeda80-94b5-11eb-94ea-59e50e56a31f.png)

# Front-End <img src="https://github.com/rafaballerini/ReactHooks/blob/master/public/React.svg.png?raw=true" width="70px" >

* ## Criando projeto Next.JS
```
$ npx create-next-app Nome-Projeto
```

* ## Instalação React / Next.JS
```
$ npm i  next react react-dom    
```
* ## Style-components
```
$ npm install --save styled-components
```
```
$  npm i -D babel-plugin-styled-components
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
```
$  npm install react-icons --save 
```
* ## React Reveall
```
$ npm install react-awesome-reveal @emotion/react --save
```
* ## Animate.css
```
$ npm install animate.css --save 
```
* ## Spline 3D
```
$ npm install @splinetool/react-spline @splinetool/runtime
```

# Back-End 💻
* ## Express
```
$ npm install express   
```
* ## TypeScript
```
$ npm typescript ts-node-dev @types/express -D 
$ npm tsc --init 
```
* ## axios
```
$ npm install --save axios   
```


# Ferramentas Extras

* [CSS Buttons](https://uiverse.io)
* [Neumorphism](https://neumorphism.io/#e0e0e0)
* [Efeito Vidro](https://css.glass/)
* [Box-Shadow CSS Generator](https://html-css-js.com/css/generator/box-shadow/)
* [FANCY-BORDER-RADIUS](https://9elements.github.io/fancy-border-radius/)

