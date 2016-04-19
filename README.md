Heroku Buildpack for Node.js and gulp.js
========================================

Usage
-----

- Set your Heroku app's buildpack URL to `https://github.com/ticketscript/heroku-buildpack-nodejs-gulp.git`. To be safe, you should really fork this and use your fork's URL.
- Run `heroku labs:enable user-env-compile` to enable environment variable support
- Run `heroku config:set GULP_TASK=build-dist` to set your gulp task to run upon deployment to `build-dist` (or any other name)
- Make sure `gulp` is in your `package.json` dependencies
- Make sure you have the `gulp` task that builds your app

Credits
-------

Inspired by [Deploying a Yeoman/Angular app to Heroku](http://www.sitepoint.com/deploying-yeomanangular-app-heroku/).

Forked from [heroku-buildpack-nodejs-gulp](https://github.com/timdp/heroku-buildpack-nodejs-gulp).

Which was forked from [heroku-buildpack-nodejs](https://github.com/heroku/heroku-buildpack-nodejs).

Heavily based on [heroku-buildpack-nodejs-grunt](https://github.com/mbuchetics/heroku-buildpack-nodejs-grunt).
