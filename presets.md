##A List of babel presets
And what they do

###.babelrc
Make sure you add the .babelrc file in your root project

````json
{
  "presets": ["es2015", "..."]
}
````

###Presets

example (with following table)
npm install
```
npm install <NPM name> --save
```
.babelrc
````json
{
    "presets": ["<Presets>", "..."]
}
````

| Presets | NPM name | Functionality |
| ------  | -------- | ------------- |
| es2015  | babel-preset-es2015 | All babel-es2015 features http://kangax.github.io/compat-table/es6/#babel |
| react   | babel-preset-react | transpiling for react jsx |

