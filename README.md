# jspm 0.17.0-beta.22 issue description

Unable to build when customizing jspm's `"directories": { "baseURL": "..." }` in `package.json`

# Issue Step by step

```bash
$ node -v
v6.2.2
$ npm -v
3.3.12
$ npm install
$ jspm -v
0.17.0-beta.22
Running against local jspm install.
$ jspm install
$ jspm build main.js
     Creating the single-file build for main.js...

err  Error: Unable to calculate canonical name to bundle file:///C:/jspm_0.17.0-beta.22/main.js. Ensure that this module sits within the baseURL or a wildcard path config.
    at getCanonicalNamePlain (C:\jspm_0.17.0-beta.22\node_modules\systemjs-builder\lib\utils.js:222:13)
    at getCanonicalName (C:\jspm_0.17.0-beta.22\node_modules\systemjs-builder\lib\utils.js:145:19)
    at C:\jspm_0.17.0-beta.22\node_modules\systemjs-builder\lib\rollup.js:283:25
    at Array.map (native)
    at C:\jspm_0.17.0-beta.22\node_modules\systemjs-builder\lib\rollup.js:282:49
```