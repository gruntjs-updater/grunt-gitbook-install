# grunt-gitbook-install
> Grunt task for installing GitBook plugins

## Getting Started
This plugin requires Grunt `~0.4.5`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-gitbook-install --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-gitbook-install');
```

*This plugin was designed to work with Grunt 0.4.x. If you're still using grunt v0.3.x it's strongly recommended that [you upgrade](http://gruntjs.com/upgrading-from-0.3-to-0.4), but in case you can't please use [v0.3.2](https://github.com/gruntjs/grunt-contrib-less/tree/grunt-0.3-stable).*


## GitBook task

_Run this task with the `grunt gitbook-install` command._

### Options

#### input
- Type: `String`
- Default: Directory of input file.

#### dest 
- Type: `String` 
- Default: (optional) Directory of output.

#### plugins
- Type: `String` (array)
- Default: none


#### Example

```js
// Gruntfile.js
grunt.initConfig({
    'gitbook-install':{
          "input": "./",
          "plugins": [
              "quizzes", 
              "exercises"
          ]
    }
});

grunt.registerTask('install', [
    'gitbook-install'
]);
```

```shell
$ grunt install
```



