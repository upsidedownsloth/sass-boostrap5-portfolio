# Follow along project - Learn Bootstrap and Sass
https://www.youtube.com/watch?v=iJKCj8uAHz8&list=PLBoFwdN-Zgdd38CE_wY6tqr1tuZZXPeSW&index=1&t=225s

## Packages required
1. Sass @ https://www.npmjs.com/package/sass
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
    ```npm install --save-dev sass```
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

#### #Before starting the project, create an npm script to complie Sass
- In package.json file, under ``"script"``, delete the pre-defined script.
- add ``"compile:sass": "sass scss:assets/css" `` 
    - Breakdown: <br>
    ``"compile:sass"`` is the name of this script. You can use any keyword. <br>
    `` "sass scss:assets/css" `` is the command 
    <br> ``sass`` is the name of the package we installed. 
    <br> ``scss``is the source of your sass file. This is where your sass file will be stored.
    <br> ``assets/css`` are the destinations where you want to keep your compiled css. Here we're telling the script to create two folders ``assets`` and ``css``
- Create a new folder called ``scss`` inside your project
- To test your script, inside the ``scss`` folder, create a sass file called ``style.scss``.
- In the terminal, ``npm run compile:sass``
- ``assets/css`` folders will be created, which will include the test ``style.scss`` file and a source map ``style.css.map``
- Note that HTML should set to ``<link rel="stylesheet" href="./assets/css/style.css">`` or something similar.
- more about <a href="https://youtu.be/iJKCj8uAHz8?list=PLBoFwdN-Zgdd38CE_wY6tqr1tuZZXPeSW&t=945">source map</a>
- Modify the script so that npm will keep watching for any changes in the Sass file and compile it in real time
<br> In the package.json file change <br> ``"compile:sass": "sass scss:assets/css" `` to <br> ``"compile:sass": "sass --watch scss:assets/css" ``

### Topic learned...
- Create package.json
- Imported and setup packages
- Watch Sass using Bash terminal
- Customising Bootstrap styling

### Web Demo
https://upsidedownsloth.github.io/sass-boostrap5-portfolio/

