# grunt-apidoc

This plugin requires Grunt `~0.4.0`

## About
Generates a RESTful API Documentation with [apidoc](http://apidocjs.com).

Generated example documentation at [http://apidocjs.com/example/](http://apidocjs.com/example/)

## Installation
1. `npm install grunt-apidoc --save-dev`
2. Add `grunt.loadNpmTasks('grunt-apidoc');` to `Gruntfile.js`

## Configuration

Add the task to your Gruntfile's **grunt.initConfig**:
```javascript
apidoc: {
  myapp: {
    src: "app/",
    dest: "apidoc/"
  }
}
```

Use only one src and one dest, apidoc search in subdirs for files with apidoc-parameters.

### Additional options

All `apidoc` options can be used within options-block, see [apiDoc examples](http://apidocjs.com/#examples) for details.

**Example options:**

**includeFilters**
With `includeFilters` you can define which files apidoc should include, default `*.js`.

**debug**
Show verbose information.

```javascript
apidoc: {
  mypp: {
    src: "app/",
    dest: "apidoc/",
    options: {
      debug: true,
      includeFilters: [ ".*\\.js$" ]
    }
  }
}
```

## Changelog

* `0.1.1` Change binary Name.
* `0.1.0` Initial release.

## License
Copyright (c) 2013 inveris OHG
Author Peter Rottmann <rottmann@inveris.de>
Licensed under the MIT license.