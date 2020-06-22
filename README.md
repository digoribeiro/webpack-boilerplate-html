# Webpack 4 Boilerplate ES6/Sass with build-in option to change preprocessor (less/stylus)
This <strong>Webpack 4 Boilerplate</strong> comes with 2 builds:

```
npm run build:dev
```
-> starts dev server on <code>localhost:8080</code> with livereload, sourcemap<br><br>

```
npm run build:prod
```
-> creates prod files to <code>/dist</code> with:

  1. compiles sass/stylus/less to css <br>
  2. autoprefixer for vendor prefixes (browser compability) <br>
  3. compiles ES6+ to ES5 <br>
  4. minifying for css/js <br>
  5. uglyfing js code <br>
  6. hash css and js file (file versioning for browser caching -> cache busting) <br>

## Setup
1. git clone https://github.com/mwieth/Webpack-4-boilerplate.git
2. run <code>npm install</code> in project folder
3. <code>npm run build:dev</code>

## Preprocessor support (default: Sass)

--> if u want to change to <strong>less</strong> run:

  1. <code>npm install less less-loader --save-dev</code>
  2. <code>npm uninstall node-sass sass-loader</code>

  3. set <code>selectedPreprocessor</code> in \webpack\loader.js to less

  4. change default files in styles from sass to less (*.less) and update <code>import</code> in index.js line 1

--> if u want to change to <strong>stylus</strong> run:

  1. <code>npm install stylus stylus-loader --save-dev</code>
  2. <code>npm uninstall node-sass sass-loader</code>

  3. set <code>selectedPreprocessor</code> in \webpack\loader.js to stylus

  4. change default files in styles from sass to stylus (*.styl) update <code>import</code> in index.js line 1

--> if u want to use the 'original' loose <strong>*.sass</strong> syntax just change the files from
*.scss to *.sass and update <code>import</code> in index.js line 1


# Webpack Boilerplate Html

>Webpack Boilerplate Html with Webpack, Stylus, and more

## Prerequisites

Make sure you have installed all of the following prerequisites on your development machine:

- Git - [Download & Install Git](https://git-scm.com/downloads).

- Node.js - [Download & Install Node.js](https://nodejs.org/en/download/)

## Cloning The GitHub Repository 

```bash
$ git clone https://github.com/digoribeiro/webpack-boilerplate-html.git
```

To install the dependencies, run this in the application folder from the command-line:

## Run Setup

```bash
$ cd webpack-boilerplate-html && npm i
```

## Run dev

```bash
$ npm run dev
```

Runs the app in the development mode.<br/>
Open [http://localhost:8000](http://localhost:8000) to view it in the browser.

The page will reload if you make edits.<br/>
You will also see any lint errors in the console.

Launches the test runner in the interactive watch mode.<br/>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

## Run Build

```bash
$ npm run build
```

## Run Prod

```bash
$ npm run Prod
```

It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the habashes.<br/>
Your app is ready to be deployed!

## Stack

- [React](https://reactjs.org/)

- [Gatsby](https://www.gatsbyjs.org/docs/)

- [Eslint](http://eslint.org/)

- [Jest](https://facebook.github.io/jest/)

- [Prettier](https://prettier.io/)

- [Prop Types](https://www.npmjs.com/package/prop-types/)

- [Styled Components](https://styled-site.com/)

As you can see, we use a lot of great tools and if you want to see more, take a look at our [package.json](package.json).

## Code Standarts

This project uses [eslint](http://eslint.org/) and [.editorconfig](http://editorconfig.org/) is defined to have indent_size of **2 spaces**.
