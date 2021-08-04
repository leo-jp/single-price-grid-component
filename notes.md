# Web Development Notes

## Getting Started
* Key notes to design efficiently
* Design-first development
* Grid System Classes
* Importing Basic Bootstrap or css styles
* Stacking divs horizontally
* Centering container
* Forcing Columns to break new-line
* Button match div size
* Sass/Scss
  * Installation and basic usage
  * Variables
* CSS
  * Fonts
  * Media Queries
  * Sticky footer
* Github

#### Key notes to design efficiently
Things noticed during web development and solutions.
* Overruse of div `rows` and `cols`. Can refactor this by simplifying by using few `rows` and `cols`.

## Design-first development 
* Familiarize & Master HTML
* Make use of design conventions like Bootstrap, SaSS, LeSS
  * Utilize grid system, flex, rows & cols, media queries
* Make data connection with VueJS, ReactJS, AngularJS
  * Utilize router, component-first, state management
* Stream data from MongoDB, MySQL, Firebase
* Refactor as needed for future website's features.
* Make use of best practices for each framework used.

## Grid System Classes
The Bootstrap grid system has [four classes](https://www.w3schools.com/bootstrap/bootstrap_grid_system.asp):

* xs (for phones - screens less than 768px wide)
* sm (for tablets - screens equal to or greater than 768px wide)
* md (for small laptops - screens equal to or greater than 992px wide)
* lg (for laptops and desktops - screens equal to or greater than 1200px wide)

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
* Follow `.container-component` class to re-align them to center.

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

## CSS
### Fonts
* [Karla](https://www.npmjs.com/package/@fontsource/karla)

### Media Queries
* Rule of thumb: to apply the style based on device's width/height, use the same structure *as is!* 
```
div.main {
  &.sub {
      // style here
  }
}

@media <condition> ( <width/height> ) {
  div.main {
    &.sub {
      // new style
    }
  }
}
```

### Sticky Footer 
* [Bootstrap v.5 sticky footer](https://getbootstrap.com/docs/5.0/examples/#custom-components): This footer does not overlap the main contents

#### Key Points for a better display of footer
  * Using [flex](https://getbootstrap.com/docs/4.0/utilities/flex/) and [flex-shrink](https://cssreference.io/property/flex-shrink/)
  * Using `footer` & `container` class
  * `d-flex flex-column`: set to vertical direction.
  * `flex-shrink-0`: element will not shrink


## Github
* [What to do when you commit to the wrong git branch](https://www.clearvision-cm.com/blog/what-to-do-when-you-commit-to-the-wrong-git-branch/)