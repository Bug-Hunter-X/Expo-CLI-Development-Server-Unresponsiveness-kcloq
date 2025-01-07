# Expo CLI Development Server Unresponsiveness

This repository demonstrates a bug encountered while using Expo CLI, where the development server becomes unresponsive, hindering development workflow.  The issue manifests as the server ceasing to respond to code changes, with minimal error reporting.

## Steps to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install` to install dependencies.
3. Start the Expo development server using `expo start`.
4. Make some changes to the code. Observe that sometimes, these changes will not be reflected in the simulator or device; the server appears to be unresponsive.

## Potential Causes

* **Memory leaks:** The Expo server might be experiencing memory leaks, leading to instability and unresponsiveness.
* **Network issues:** Intermittent network problems may affect communication between the server and the client.
* **Conflicting packages:**  Incompatibilities or conflicts between packages can disrupt server functionality.
* **Expo CLI version:** Older versions may have underlying issues that have been addressed in newer releases.

## Solution

The solution involves restarting the server.  If the issue persists, consider upgrading Expo CLI or exploring alternative solutions, such as increasing the system's memory allocation.