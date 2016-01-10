# babel-6-installation-guide
How to actually use babel 6

##Why?
Babel 6 is a confusing tool, this guide shows you the steps you need to make it work..
You always need a .babelrc file in the root of your project

##.babelrc (Must have)
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

##Babel require hook
To develop using babel node, you can
```
npm install --save babel-register
```
