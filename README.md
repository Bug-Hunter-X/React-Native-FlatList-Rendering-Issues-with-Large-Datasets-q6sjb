# React Native FlatList Rendering Bug

This repository demonstrates a common bug in React Native's FlatList component when dealing with large datasets.  The bug manifests as incorrect rendering or failure to update component states, leading to visual glitches or unexpected behavior.

## Bug Description
When using FlatList with a significant number of items, some components may render incorrectly or fail to update their state correctly due to issues with key assignment and component lifecycle management.

## Reproduction
1. Clone this repository.
2. Run `npm install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`.
4. Scroll through the FlatList. Observe rendering inconsistencies.

## Solution
The solution involves ensuring proper key assignment to each item in the FlatList, utilizing the `keyExtractor` prop.  Additionally, optimization techniques like `getItemLayout` can improve performance.

See `bugSolution.js` for a corrected implementation.