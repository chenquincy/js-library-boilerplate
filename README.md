## js-library-boilerplate

This is a boilerplate for developing npm library.



### Start

1. clone this repo and remove `.git` folder
2. search `your-library-name` in `package.json` and change them all to your library name
3. If your npm module support to import by `script` element , change the `YourLibraryName` (at `package.json -> scripts -> build:browser `) to the variable that your want to use in browser, or your can delete the `build:browser` script.
4. write your code in `src` folder (support ES6 and ES7)



### Build

#### build npm module

``` shell
npm run build # compile your code from ES6/ES7 to ES5, output to lib folder.
```

#### build browser module

``` shell
# compile your code and output as dist/your-library-name.js, your can import it by script element.
npm run build:browser
# compile and output the mini version as dist/your-library-name.min.js
npm run dist
```

