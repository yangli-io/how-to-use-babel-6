# babel-6-installation-guide
How to actually use babel 6

* [.babelrc (must have for every project)](#babelrc)
* [Babel for the Server](#babel-for-the-server)

##Why?
Babel 6 is a confusing tool, this guide shows you the steps you need to make it work..
You always need a .babelrc file in the root of your project

##<a name="#babelrc"></a>.babelrc (Must have)
You will need some presets, at the very least you will need the es2015 preset for es6/es2015. Heres a list of all [babel-es6 features](http://kangax.github.io/compat-table/es6/#babel)

* Heres a list of presets and what they do [link](https://github.com/yangli1990/how-to-use-babel-6/blob/master/presets.md);

```
npm install --save babel-preset-es2015
```
````json
{
  "presets": ["es2015"]
}
````

##<a name="babel-for-the-server"></a>Babel for the Server
* You can either use babel-register or babel-node
* make sure you have .babelrc

###Require Hook
To develop using babel node, you can
```
npm install --save babel-register
```

In your entry file
entry.js
````javascript
require('babel-register');
require('index.js');
//Require any other files
````

[babel official documentation](https://babeljs.io/docs/setup/#babel_register)

###Babel-node
This adds a babel-node command
```
npm install --save babel-cli
```

In your terminal

for npm 3
```
./node_modules/.bin/babel-node index.js
```

for npm 2 and older
```
./node_modules/babel-cli/bin/babel-node index.js
```
