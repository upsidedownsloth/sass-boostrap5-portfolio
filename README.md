# Follow along project - Learn Boostrap and Sass
https://www.youtube.com/watch?v=iJKCj8uAHz8&list=PLBoFwdN-Zgdd38CE_wY6tqr1tuZZXPeSW&index=1&t=225s

## Packages required
1. Dart-Sass @ https://www.npmjs.com/package/sass
2. Bootstrap5 @ https://getbootstrap.com/
3. Font Awesome @ https://fontawesome.com/
4. Autoprefixer @ https://www.npmjs.com/package/autoprefixer

#### 1. Create package.json file
```npm init```

#### 2. Sass Setup
- go to www.npmjs.com
- look for 'sass'
- Go to 'Usage'
    - This project will use npm command as we have initilised npm
    ```npm --save-dev-sass```
    - Once installed, a folder named 'node_modules' will be created in the project folder. This is where the project will keep all sass file.

#### 3. Get Bootstrap
- https://getbootstrap.com/
- install via npm ``npm install bootstrap --save``
    including ``--save`` to save it to dependecies in package.json

#### 4. Font Awesome
- get fron awesome via npm
- https://fontawesome.com/v5.15/how-to-use/on-the-web/setup/using-package-managers
- ``npm install --save @fortawesome/fontawesome-free``

#### 5. Autoprefixer
- Is a pugin to parse CSS and add vendor prefixes to CSS rules
- https://github.com/postcss/autoprefixer#readme
- use the post-cli to run Autoprefixer from CLI
- ``npm install postcss-cli autoprefixer --save`` (only this line and flag it with ``--save``)

### Topic learned...
- Create package.json
- Imported and setup packages
- Watch Sass using Bash terminal
- Customising Boostrap styling

### Web Demo
https://upsidedownsloth.github.io/sass-boostrap5-portfolio/

