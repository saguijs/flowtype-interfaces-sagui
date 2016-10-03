# flowtype-interfaces-sagui

# This package is deprecated. As of v7.0.0-rc.1, Sagui itself contains the flowtype interface for Jasmine

Flowtype interface declarations for the built-in [Sagui](https://github.com/saguijs/sagui) test utilities.

## Why

The purpose of this repo is to group Flowtype declarations meant to be loaded automatically in the `.flowconfig` as `libs` in Sagui bootstrapped projects. The main reason not to use the [larger repository Flow-typed](https://github.com/flowtype/flow-typed) is that the vast majority of the type declarations in there are not needed by Sagui installations.

Type declarations for the Sagui-bundled testing tools ([Jasmine](http://jasmine.github.io/), [Sinon](http://sinonjs.org/)) are also done in a very liberal way so that no Jasmine structure related errors are thrown by the type checker. The reasoning behind this is that the intent of type checking the test code is to verify the types involved in the actual example content, not of the ones related to the testing tool (such as the `describe` and `it` functions).

## License

ISC License.
