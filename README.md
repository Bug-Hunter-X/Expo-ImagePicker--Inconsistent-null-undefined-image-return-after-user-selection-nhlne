# Expo ImagePicker: Null/Undefined Image Return Bug

This repository demonstrates a bug in Expo's ImagePicker library where the selected image URI can be unexpectedly null or undefined even after successful user selection.  The issue appears inconsistent, making debugging challenging.  This repo provides example code illustrating the problem and a potential solution.

## Reproducing the Bug

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app using Expo Go or a similar Expo client.
4. Select an image from the picker.  Observe that the image URI may sometimes be null or undefined despite a successful selection.

## Potential Solution

The provided `bugSolution.js` file offers a possible fix that utilizes promises and asynchronous handling to ensure proper image retrieval before proceeding with further operations.  However, this solution isn't guaranteed to work in all scenarios.  More robust approaches might be needed depending on the specific implementation and potential race conditions within Expo's ImagePicker.