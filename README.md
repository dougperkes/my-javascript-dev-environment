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
8. Testing and continuous integration framework - Lots of choices is to just pick a framework and run with it. Also need an assertion library. Assertion is a way to declare what you expect.
  1. Unit test with #Mocha#
  2. Assertion Librayr with Chai
  3. JSDom as a helper library
  4. Browser simulation via in-memory DOM with JSDOM.
  5. Where to put the tests? Put the test right next to the file being tested. Name with either filename.spec.js or filename.test.js.
  6. Run tests every time you hit save. Units tests *should* be fast because they don't hit external resources.
  7. Continuous Integration with TravisCI.
