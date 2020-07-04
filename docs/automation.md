# Automation frameworks

1. Grunt
   1. the "original"
   2. Configuration over code
   3. Writes intermediate files between steps, then reads back from them
   4. Been around a long time so has a large plugin ecosystem

2. Gulp
   1. Newer
   2. Uses in-memory streams to pipe from one task to the next (no files)
      1. Result - typically faster than Grunt
   3. Code over configuration
      1. you use a code-based gulp.js file to configure it
   4. Been around a while and large plugin ecosystem

3. npm scripts
   1. Declared in package.json
   2. Leverage your OS command line
   3. Directly use npm packages
   4. Can call seaparate node scripts if needed
   5. convention-based pre/post hooks
   6. Leverage the world's largest package manager
   7. Why?
      1. Use tools directly
      2. No need for separate plugins
         1. Which can have bugs... more abstraction
         2. Eliminate extra dependencies in the tools
      3. simpler debugging
      4. better docs - unified docs
      5. easy to learn
      6. simple
   8. [Read more about why on this web page](bit.ly/npmvsgulp)
   9. **NOTE:** "standard" npm scripts, like "start" can be run with `npm start`, but any script with a custom name must be run with `npm run <script_name>`. The standard lifecycle scripts can also be run with the `npm run` command.
