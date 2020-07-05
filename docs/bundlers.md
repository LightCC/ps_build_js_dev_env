# Description

Modules are ways to import javascript code from outside a given file/module.

These module formats were available prior to ES6:
1. IIFE
2. AMD - Asynchronous Module Definition
3. CJS - CommonJS (Node.js type)
4. UMD - Universal Module Definition (UMD) - combine AMD and CJS

Then  with ES6:
5. ES6 Modules
   1. These require being statically analyzable
      1. Allows them to be known at compile time - imports cannot change dynamically at run-time)
      2. Allows linting and static analysis to find common code errors

# Bundlers

Bundlers package and/or repackage code so it is organized better for production. For example, it might reorganize code so the JS files match up with each HTML page so that only the code needed at that time needs to be downloaded for faster startup.

Popular bundlers include:
1. Browserify
   1. It was the original, helped popularize npm packages
   2. Bundles npm packages for the web
   3. large plugin ecosystem
2. Webpack
   1. Bundles more than just JS
   2. Has bundle splitting
   3. Import CSS, images, etc., the same as JS
   4. Built in hot-reloading web server (for all file types)
   5. Webpack 2 is coming soon and has tree shaking (probably out by 2020!)
3. Rollup
   1. Tree shaking (minimizes sizes)
   2. Faster loading production code
   3. Quite new (2016)
   4. Great for library authors
   5. No hot relading and code splitting yet
4. JSPM (JavaScript package manager)
   1. Uses SystemJS behind the scenes, a universal module loader
   2. Can load modules at runtime
   3. Has its own package manager
   4. Can install from npm or git
   5. Uses rollup as a plugin
