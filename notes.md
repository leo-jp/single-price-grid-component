# Web Development Notes
Things noticed during web development and solutions.
* Overruse of div `rows` and `cols`. Can refactor this by simplifying by using few `rows` and `cols`.

## Design-first development 
* Familiarize & Master HTML
* Make use of design conventions like Bootstrap, SaSS, LeSS
  * Utilize grid system, flex, rows & cols
* Make data connection with VueJS, ReactJS, AngularJS
  * Utilize router, component-first, state management
* Stream data from MongoDB, MySQL, Firebase
* Refactor as needed for future website's features.
* Make use of best practices for each framework used.

## Importing Basic Bootstrap or css styles
##### Inside Header
```
  <link rel="stylesheet" href="<path>/bootstrap/dist/css/bootstrap.min.css"/>
  <link rel="stylesheet" href="<path>/bootstrap/dist/css/bootstrap-grid.min.css"/>
```
##### Inside Body
```
  <script source="./node_modules/bootstrap/dist/js/bootstrap.bundle.min.js"></script>
  <script source="./node_modules/bootstrap/dist/js/bootstrap.min.js"></script>
```

## Stacking divs Horizontally
* Use `container-fluid`

## Centering container
* prerequisite: `container-fluild`
* Place `justify-content-center` on `.row` classes to re-align them to center.

## Forcing columns to break to new line
* `<div class="w-100"></div>`

## Button match div size
* Use `btn-block`

## Sass/Scss
### [Installation and Basic Usage](https://webdesign.tutsplus.com/tutorials/watch-and-compile-sass-in-five-quick-steps--cms-28275)
* `npm install sass` or `yarn add sass`
* add these to `package.json`
```
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1",
    "scss": "node-sass --watch styles/scss -o styles/css"
  }
```
1. `node-sass`: Refers to the node-sass package.
2. `--watch`: An optional flag which means “watch all .scss files in the scss/ folder and recompile them every time there’s a change.”
3. `styles/scss`: The folder name where we put all our .scss files.
4. `-o styles/css`: The output folder for our compiled CSS.
* To compile and run: `npm run scss` or `yarn run scss`

### Variables
* [Maps](https://sass-lang.com/documentation/values/maps)

## Fonts
* [Karla](https://www.npmjs.com/package/@fontsource/karla)