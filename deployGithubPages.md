## Tutorial seguido para deploy en github pages

https://www.youtube.com/watch?v=NO42F_urRec

`npm install -g gatsby-cli`

`gatsby -v` --> Comprobar instalacion version de gatsby

gatsby new anbreakerPortFolioGatsby https://github.com/LekoArts/gatsby-starter-portfolio-cara

`gatsby develop` or `npm start develop` --> http://localhost:8000/

`gatsby build` --> Para montar el proyecto

`gatsby serve` --> http://localhost:9000/

dependencias para github pages --> `npm i gh-pages`

### Configuracion de archivos gatsby-config.js && package.json

gatsby-config.js

-   `module.exports = { // Agregado nombre repo Github pathPrefix: 'anbreakerPortFolioGatsby',`

package.json

-   `//agregar siguiente script para desplegar en github pages:`"scripts": {"deploy":"gatsby build --prefix-paths && gh-pages -d public"`

### Prueba de funcionamiento de deploy en local:

-   `npm run deploy`
