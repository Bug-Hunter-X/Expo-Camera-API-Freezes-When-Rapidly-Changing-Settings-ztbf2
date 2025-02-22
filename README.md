# Expo Camera API Freezing Bug

This repository demonstrates a bug in the Expo Camera API where rapidly changing camera settings (such as `flashMode` or `autoFocus`) can cause the camera preview to freeze or become unresponsive.  This issue affects both Android and iOS platforms. 

## Bug Reproduction

The `bug.js` file contains code to reproduce the issue.  Run the Expo app and rapidly toggle the flash or autofocus settings.  You should observe the camera preview freezing or becoming unresponsive. 

## Solution

The `bugSolution.js` file provides a potential solution involving debouncing the setting changes to prevent rapid calls to the camera API. This approach ensures that changes only occur after a certain delay, avoiding race conditions or resource contention within the Camera API.

## Contributing

Contributions to refine the solution or find alternative approaches are welcome!