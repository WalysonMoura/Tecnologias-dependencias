
# 🛠️ Tecnologias/Ferramentas ultilizadas

* ### NPM  de instalação das tecnologias mais usadas por mim

![mock1](https://user-images.githubusercontent.com/71772559/113493479-eceeda80-94b5-11eb-94ea-59e50e56a31f.png)


<details>
 <summary><h2>Config GIT</h2></summary>

  
```bash

[user]
    name = WalysonMoura
    email = walysonmoura222@gmail.com

[includeIf "gitdir:C:/Users/Vaio/www/programacao/redacao-ia/"]
  path = C:/Users/Vaio/www/programacao/redacao-ia/.gitconfig-redacao-ia

[includeIf "gitdir:C:/Users/Vaio/www/programacao/agencia-upcoder/"]
  path = C:/Users/Vaio/www/programacao/agencia-upcoder/.gitconfig-agencia-upcoder

[core]
  editor = code --wait

[alias]
  s = !git status -s
  c = !git add --all && git commit -m
  l = !git log --pretty=format:'%C(blue)%h%C(red)%d %C(white)%s - %C(cyan)%cn, %C(green)%cr' 
```
</details>


<details>
 <summary><h1>Front-End <img src="https://github.com/rafaballerini/ReactHooks/blob/master/public/React.svg.png?raw=true" width="70px"/></h1>
 </summary>

* ## Instalação React / Next.JS / Styled-Components

```bash
npm create next-app
```

* ## Style-components

```bash
npm i styled-components --save
```

```bash
npm i  -D babel-plugin-styled-components
```

 Para utilizaçâo do Styled Components com Next é necessário a criação do arquivo `babel.config.js` na raiz do projeto com as configurações a seguir:  

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

```bash
  npm i  react-icons --save 
```

* ## React Reveall

```bash
npm i  react-awesome-reveal @emotion/react --save
```

* ## React Tilt [site](https://mkosir.github.io/react-parallax-tilt/?path=/story/react-parallax-tilt--default)

```bash
npm i  react-parallax-tilt
```

* ## Animate.css

```bash
npm i  animate.css --save 
```

* ## Spline 3D

```bash
npm i  @splinetool/react-spline @splinetool/runtime
```

<details>
<summary><h2>Ferramentas Extra</h2></summary>

* [CSS Buttons](https://uiverse.io)
* [Neumorphism](https://neumorphism.io/#e0e0e0)
* [Efeito Vidro](https://css.glass/)
* [Testes](https://www.refraction.dev/)
* [Box-Shadow CSS Generator](https://html-css-js.com/css/generator/box-shadow/)
* [FANCY-BORDER-RADIUS](https://9elements.github.io/fancy-border-radius/)

</details> 

</details>

<details>
 <summary><h1>Back-End 💻</h2></summary>

<details>
 <summary><h2>ambiente Node.js</h2></summary>

```bash
 npm init -y   
```
* ## All

```bash
 npm i typescript  @types/node tsup vitest  eslint tsx -D   
```

* ## TSX

```bash
 npm i tsx -D   
```

* ## TypeScript

```bash
npm add typescript  @types/node -D 
```

* ### Configuração do TypeScript

```bash
 npx tsc --init
```

```.json
 {
   "target": "es2020",  
   
   "baseUrl": "./",                                     /* Specify the base directory to resolve non-relative module names. */
    "paths": {
      "@/*": ["./src/*"]
    },
 }
```



* ## compilar  TypeScript

```bash
pnpm i ts-node-dev -D
```

## compilar TypeScript (Build)

* ###  tsup

```bash
npm i tsup -D
```

* ## ESlint

```bash
 npm i eslint -D   
```

```bash
 npm init @eslint/config 
```

```bash
 npm i @rocketseat/eslint-config -D   
```

```bash
 npm i eslint-plugin-vitest-globals -D   
```

 arquivo `.eslintrc.json`

```.json
 {
   "extends": [
     "@rocketseat/eslint-config/node",
     "plugin:vitest-globals/recommended"
   ],
   "rules": {
    "no-useless-constructor": "off",
    "no-new": "off"
   },
   "env": {
    "vitest-globals/env": true
  }
 }
```

arquivo `.eslintignore`

```.eslintignore
 node_modules
 build
```

  ```.json
 {
   "scripts": {
     "start": "tsx src/server.ts",
     "lint": "eslint src --ext .ts --fix",
     "dev": "tsx watch src/server.ts",
     "build": "tsup src",
     "test": "viteste"
   }
 }
 ```

* ## dotenv

```bash
 npm i dotenv   
```

* ## .npmrc
`.npmrc`
```bash
save-exact=true  
```


</details>

<details>
 <summary><h2>Framework</h2></summary>

* ###  Express
  
    ```bash
     npm i express   
    ```

    ```bash
     npm i  @types/express -D 
    ```
  
* ###  Fastify
  
    ```bash
     npm i fastify  
    ```

    ```bash
     npm i  @fastify/cookie
    ```
  
* ###  Nest.JS
  
   ```bash
    pnpm  
   ```

   ```bash
     pnpm
   ```

</details>

<details>
 <summary><h2>Testes</h2></summary>

* ###  Viteste

 ```bash
  npm i vitest -D
 ```
 `vite.config.js`

```typescript
  import { defineConfig } from 'vitest/config'
import tsconfigPaths from 'vite-tsconfig-paths'

export default defineConfig({
  plugins: [tsconfigPaths()],
  test: {
     globals: true,
    environmentMatchGlobs: [['src/http/controllers/**', 'prisma']],
  },
})

 ```

  `tsconfig.json`

```json
  "types": [
      "vitest/globals"
    ]

 ```
</details>

<details>
 <summary><h2>Docker</h2></summary>

* ###  Docker Composer
`docker-compose.yml`

 ```yml
  version: '3'
    services:
      api-solid-pg:
        image: bitnami/postgresql
        ports:
          - 5432:5432
        environment:
          - POSTGRESQL_USERNAME=docker
          - POSTGRESQL_PASSWORD=docker
          - POSTGRESQL_DATABASE=apisolid
      
 ```

 ```bash
  docker compose up -d
 ```

# Comandos Docker

- Com esse comando você verifica todos os containers ativos (e não ativos com o comando `-a`)
```javascript
 docker ps -a
```


```javascript
 docker ps -a
```


```javascript
 docker start nome_do_container
```

- O comando `run` cria um novo container e logo após você especifica o nome da imagem que o mesmo vai utilizar (no exemplo a a imagem `hello-world`)
```javascript
 docker run hello-world
```

- O comando `-it` especifica que o container (no exemplo a a imagem `hello-world`) após ser criado deverá ficar ativo e executar com o comando `bash`
- Com o comado `--rm`  o container deverá ser excluido após executado
```javascript
  docker run -it --rm ubuntu:latest bash
```

### Nginx

```javascript
  docker run nginx 
```
- Por padrão o nosso container criado com a imagem do Nginx utiliza a porta 80
- com o comando `-p 8080:80` utlizamos um redirecionamento da porta que o container está utilizando com alguma porta da nossa máquina, assim podemos acessar a porta do nosso Container 
- o comando `-d` é possivel utilizar o terminal, e o processo do contaneir será executado sem bloquear o terminal
```javascript
  docker run -d -p 8080:80 nginx
```

### Remover containers
- Utilize o comando `rm` com ID do container

```javascript
  docker rm 07f933bceeef
```

</details>




<details>
 <summary><h2>ORM</h2></summary>

* ###  Prisma
 
```bash
 npm i -D prisma
```

```bash
 npm i @prisma/client
```

#### Iniciando Database

```bash
 npx prisma init --datasource-provider sqlite
```

#### Criando Migrations

 ```bash
 npx prisma migrate dev
```

#### Prisma Studio

```bash
 npx prisma studio
```

#### Gerador de diagrama de relacionamento com entidades Prisma

```bash
 npm i -D prisma-erd-generator @mermaid-js/mermaid-cli
```

Cole esse código no arquivo  `schema.prisma` :

 ```.js
 generator client {
  provider = "prisma-client-js"
  output   = "./generated/prisma-client-js"
}
 ```

 ```bash
 npx prisma generate
```
  <details>
    <summary>
       <h4>Prisma Client com o Next.js</h4>
    </summary>

 ```.ts
   import { PrismaClient } from '@prisma/client'

const prismaClientSingleton = () => {
  return new PrismaClient()
}

declare global {
  var prismaGlobal: undefined | ReturnType<typeof prismaClientSingleton>
}

const prisma = globalThis.prismaGlobal ?? prismaClientSingleton()

export default prisma

if (process.env.NODE_ENV !== 'production') globalThis.prismaGlobal = prisma
  ```
  </details>
  
</details>


<details>
 <summary>
   <h2>SQL Query Builder</h2>
 </summary>

* ###  Knex.js

 ```bash
   npm install knex sqlite3
 ```

</details>




