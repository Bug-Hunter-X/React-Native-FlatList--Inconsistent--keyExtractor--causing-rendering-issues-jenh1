# React Native FlatList KeyExtractor Bug

This repository demonstrates a common error in React Native's `FlatList` component: using an inconsistent or invalid `keyExtractor` function.

The `keyExtractor` function is crucial for `FlatList` to identify and update items efficiently.  Failure to provide unique keys leads to unpredictable rendering behavior, such as missing or duplicated items, or items appearing in the wrong positions.

The `bug.js` file showcases the problematic code. The `bugSolution.js` file shows the corrected version with a properly implemented `keyExtractor` function.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run the app on an emulator or physical device.
4. Observe the incorrect rendering in `bug.js` and the corrected rendering in `bugSolution.js`.

## Solution

Ensure your `keyExtractor` function always returns unique and consistent keys for each item in your data array.  Using the item's unique ID is the most reliable approach.