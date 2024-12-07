# React Native: TypeError: Cannot read properties of undefined (reading '...')

This repository demonstrates a common error in React Native: `TypeError: Cannot read properties of undefined (reading '...')`. This occurs when attempting to access a property of an object that is null or undefined.  The example showcases this issue and provides a solution.

## Bug Description

The bug arises from accessing properties of an object before it's properly populated with data (often during asynchronous operations) or when a component's state or props haven't been updated yet. This is a frequent problem when dealing with data fetched from APIs or during the component lifecycle.

## Bug Reproduction

The `bug.js` file shows the problematic code.  Run the app and observe the error in the console.

## Solution

The `bugSolution.js` file demonstrates how to fix this using optional chaining and nullish coalescing operators. These prevent the error by gracefully handling the case where the object or property is undefined.

## How to Run

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app on an emulator or device.
