# Babel Learnig

### Transpiling es6 JS syntax and Typescript to es5 syntax.

> **Steps:**
>
> 1.  Install all dependencies:
>     - @babel/cli
>     - @babel/core
>     - @babel/preset-env
>     - @babel/preset-typescript
>     - typescript
>     - rimraf
> 2.  Create **.babelrc** file
>     - Include all the preset & plugins
>       > {
>       > "presets": ["@babel/preset-env", "@babel/preset-typescript"]
>       > }
> 3.  Run `npm run tsc -- --init` to generate **tsconfig.json** file and enable or disbale the flags as per need, can refer to tsconfig file in project dir.
> 4.  Add following code in **package.json**
>     >           "scripts": {
>     >               "transpile": "rimraf build/ &&  tsc",
>     >               "start": "npm run transpile",
>     >               "dev": "ts-node-dev --respawn --transpile-only --no-notify typescript/index.ts",
>     >           }

### To run the project.

> **Steps:**
>
> 1. `npm install`
> 2. `npm start` -- can check build folder for transpiled code.
> 3. `npm run dev` -- to start server
