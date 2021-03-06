# prop-types-callable

This is a fork of React [`prop-types`](https://github.com/reactjs/prop-types), intended for use in production.

## Differences

The main difference is that all validator functions are manually callable, in both development and production environments, without any warnings.

- Updated environment checks and tests to allow calling validator functions
- Expose `PropTypeError`, a light-weight implementation of native Error object without stack trace
- Expose only babel transpiled source files, instead of a browserify build
