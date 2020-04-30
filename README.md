# React Navigation 1.5.11 (w/ React 16.6+ Support)

This is a fork of the final version of React Navigation 1 that has been slightly modified to work with React 16.6+ (the version where React Hooks were introduced). The problem is that some React Components are now returned as objects instead of functions or classes, which causes a validation check to fail with the error message: `"Error: The component for route '...' must be a React component. For example: ..."`.

This branch updates the validation class to support these new components, such as `{$$typeof: 'Symbol(react.memo)', ...}` which is returned by Redux connected components in React 16.6+.

### Documentation

[https://reactnavigation.org/docs/en/1.x/getting-started.html](https://reactnavigation.org/docs/en/1.x/getting-started.html)

### Deprecation Warning

Note that React Navigation v1.x is no longer supported. You should absolutely avoid using this in new React Native applications unless you have a good reason.

Here are some alternatives:

1. [React Navigation 4](https://reactnavigation.org/docs/en/getting-started.html)
2. ...or, even better, Wix's [react-native-navigation](https://wix.github.io/react-native-navigation) library.
