# standard-summary

This CLI module displays output from [standard](http://npm.im/standard) as a list of style errors, ordered by count.

For alternative formats, see [standard-tap](http://npm.im/standard-tap), [standard-json](http://npm.im/standard-json), and [standard-reporter](http://npm.im/standard-reporter).

## Installation

Install standard and standard-summary globally with npm:

```sh
npm install standard standard-summary --global
```

## Usage

`cd` into your favorite javascript project, then pipe the output of `standard` into `standard-summary`:

```
$ cd my/project
$ standard | standard-summary

5966   Extra semicolon
1615   Missing space before function parentheses
318    Strings must use singlequote
55     Return statement should not contain assignment
38     Expected { after 'if' condition
24     Expected '===' and instead saw '=='
23     Missing '()' invoking a constructor
17     Block must not be padded by blank lines
16     Unexpected trailing comma
13     Multiple spaces found before '+='
12     The '__proto__' property is deprecated
10     Expected space(s) after "catch"
...
```

## Tests

```sh
npm install
npm test
```

## Dependencies

- [concat-stream](https://github.com/maxogden/concat-stream): writable stream that concatenates strings or binary data and calls a callback with the result
- [pad](https://github.com/wdavidw/node-pad): Left and right string padding

## Dev Dependencies

None

## License

MIT

_Generated by [package-json-to-readme](https://github.com/zeke/package-json-to-readme)_
