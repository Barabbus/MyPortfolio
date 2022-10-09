Responsive website built using HTML, SASS, Flex, CSS Grid, Javascript, node.js and hosted on Github Pages.  Uses Google fonts and Font Awesome.

We're using node-sass which compiles scss files down to regular css files (main.css) that the browser can read.

main.scss is the main sass file, with _config, _menu and _mobile scss files as partials imported into main.scss.

We create a sass script in package.json to run node-sass:  "node-sass -w scss/ -o dist/css/ --recursive"  run node-sass and watch the main.scss folder and output the compiled sass to dist/css.  --recursive is added to deal with possible issues of having partial scss files and autoreload.  The sass is then compiled to the main.css folder in dist/css/ in minified form.