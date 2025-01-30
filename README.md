# React useState Bug: Null Object Access

This repository demonstrates a common error when using the `useState` hook in React: attempting to access a property of a potentially null object before the state has been properly initialized.

## Bug Description
The `MyComponent` component initializes its state to `null`. The `incrementCount` function then tries to increment `state.count`, which will throw an error if `state` is still `null` when the function is called.

## Solution
The solution involves providing a default value for `state.count` in the initial state or using optional chaining to safely access the property.