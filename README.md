<p align="center">
  <img src="assets/img/logo.svg" width="100">
</p>

# Front-end Week 2k18

[Access the website](http://frontendweek.com.br/)

This project uses:
- [Pug](https://pugjs.org/)
- [Sass](http://sass-lang.com/)
- [Grunt](https://gruntjs.com/)
- [Browsersync](https://www.browsersync.io/)

## Getting Started

### Installation

First of all, install the dependencies to run this boilerplate.

- [NodeJS](http://nodejs.org/)
- [Grunt](https://gruntjs.com/)

```sh

# Clone this repository
git clone git@github.com:frontendweek/frontendweek-website.git
cd frontendweek-website.git

# install dependencies
npm install

```

After that, you should be good to go :)

### Folders/Files Structure

```sh
├── assets/
│   ├── css/
│   │   └── *.sass
│   ├── img/
│   ├── js/
│   │   ├── modules/
│   │   └── index.min.js
├── includes/
│   └── *.pug
├── Gruntfile.js
├── index.pug
├── package.json
├── README.md
```
These structure will change during the project.


### Tasks

- `grunt concat`: concat `modules/*.js` into `index.min.js`
- `grunt uglify`: uglifies `index.min.js` into itself

- `grunt sass`: build [everything].sass into style.css
- `grunt autoprefixer`: adds vendor prefixes to style.css

- `grunt imagemin`: optimize `*.jpg`,`*.png`,`*.svg` inside `assets/img`

- `grunt pug`: generates `index.html` from `index.pug` + `includes/*.pug`

- `grunt compile`: run concat, uglify, sass, autoprefixer, imagemin, pug; does *not* start server
- `grunt`: run watch [tasks: pug, sass, concat] and start BrowserSync local server


## License

MIT License