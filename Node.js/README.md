# Node.js

## Install [Node.js](http://nodejs.org/) with [nvm](https://github.com/creationix/nvm) (Node Version Manager):

#### Install nvm

    $ brew install nvm

#### Install Nodejs via nvm

    $ nvm  # check the nvm use message
    $ nvm install stable  # install most recent nodejs stable version
    $ nvm ls  # list installed node version
    $ nvm use stable  # use stable as current version
    $ nvm ls-remote  # list all the node versions you can install
    $ nvm alias default stable  # set the installed stable version as the default node

Node modules are installed locally in the `node_modules` folder of each project by default, but there are at least three that are worth installing globally. Those are [Grunt](http://gruntjs.com/), [Gulp](http://gulpjs.com/), and [Bower](http://bower.io/):

    $ npm install -g grunt-cli
    $ npm install -g gulp
    $ npm install -g bower

## Npm usage

To install a package:

    $ npm install <package> # Install locally
    $ npm install -g <package> # Install globally

To install a package and save it in your project's `package.json` file:

    $ npm install <package> --save

To see what's installed:

    $ npm list # Local
    $ npm list -g # Global

To find outdated packages (locally or globally):

    $ npm outdated [-g]

To upgrade all or a particular package:

    $ npm update [<package>]

To uninstall a package:

    $ npm uninstall <package>
