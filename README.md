# ls-cordova-plugins

[![Build Status][travis-image]][travis-url]

> List Cordova plugins

Greps through `package.json` and prints a space-delimited list of dev
dependencies that contain a `cordova-plugin-` prefix. Takes one optional
argument that prepends a string to each result.

Intended to be used with the local directory variant `cordova plugin add` so
that plugins can be installed within the project's top-level `node_modules` and
can thereby be cached by TravisCI.

[travis-image]: https://img.shields.io/travis/tlvince/ls-cordova-plugins.svg
[travis-url]: https://travis-ci.org/tlvince/ls-cordova-plugins

## Usage

```shell
ls-cordova-plugins [prefix]
```

## Examples

Prepend `node_modules`:

```shell
ls-cordova-plugins node_modules/
# =>
# node_modules/cordova-plugin-crosswalk-webview node_modules/cordova-plugin-device
```

## Author

© 2015 Tom Vincent <npm@tlvince.com>

## License

Released under the [MIT License](http://tlvince.mit-license.org).
