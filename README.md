# fast-node
# Step-by-step.
# Create your Project.
 
 * Open the ``vsCode`` app.
 * Open Command Line ```ctrl+shift+`~``
 * create a new folder ``mkdir`` your folder_name.
 * ``cd`` to your folder_name.
 
 # Create your Project file.
 * In your Command line verify if ``npm`` is installled with this command ``npm -v``

* Initialize your **Node.js** project:`$ `` npm init -y`
* Install **express.js**: `$:``install i express --save`

* Create a new project file `$: ``touch index,js`
* Open your project file`index.js` in **vsCode**

# Edit your package.json
```
"scripts:{
    "test": "echo \ "Error: no test specified\" && exit 1",
    "start": "node index.js"
},

```

* Create a ~~.gitignore~~ file: `$``echo 'node_modules' >> .gitignore
* Copy and paste the **Code** into the **index.js**

```
const express = require('express');
const app = express();

app.get('/', function(req, res){

    res.send('<h3>Hello Node on Heroku</h3>');
});
app.listen(process.env.PORT || 3000);

```
# Testing Your New App.

* On your terminal run the following ``node index.js``
* Navigate to your browser of choice and type ``localhost:3000``


# Heroku App

* Navigate to https://www.heroku.com/

* Create `new app`
* Select name for your app.**(with uniqure identifier)**
* Click on the purple ``Create App``button
* Link app to yout ``GitHub``
* Select your ``repo``
* **Bingo** your got a `super_awsome app`
