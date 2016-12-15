# my-javascript-dev-environment
A sample javascript dev starter kit based on Cory House's pluralsight course (https://app.pluralsight.com/library/courses/javascript-development-environment)

1. .editorconfig
2. npm for package management with default package.json
3. express as development web server. Run the following: `node buildScripts/srcServer.js`
    1. localtunnel for work-in-progress running on local machine with public url. Just run the following script: `lt --port 3001`
4. Automation with npm scripts (Grunt < Gulp < npm scripts). npm scripts declared in package.json and can directly use npm packages and convention-base pre/post hooks. Run `npm start`. Support for running tasks in parallel. 
5. Babel as the transpiler via dedicated .babelrc file and using babel-node in npm scripts to do automatic transpiles.
6. Bundling via Webpack and using ES6 Modules (CSS, Images, Fonts, HTML) and supports Bundle splitting and debugging via sourcemaps.
7. Linting via ESLint.
