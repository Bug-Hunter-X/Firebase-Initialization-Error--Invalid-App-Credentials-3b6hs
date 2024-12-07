# Firebase Initialization Error: Invalid App Credentials

This repository demonstrates a common error encountered when initializing Firebase: `The provided app credentials are invalid`. This error typically arises from incorrect configuration of your Firebase project or firebaseConfig object.

## Steps to Reproduce

1. Clone this repository.
2. Run the `bug.js` file.  You'll observe the error message.
3. Refer to `bugSolution.js` for the corrected code and steps to resolve the issue.

## Solution

The solution involves double-checking your Firebase configuration:

1. **Verify Firebase Console Configuration:**
    * Ensure your project is correctly set up in the Firebase console.
    * Correctly add the `apiKey`, `authDomain`, `projectId`, `storageBucket`, `messagingSenderId`, `appId`, and `measurementId` to your `firebaseConfig` object.
2. **Check for Typos:**
    * Carefully review your `firebaseConfig` object for typos in keys or values. A single incorrect character can cause this error.
3. **Confirm API Key Validity:**
    * Make sure your API key is valid and hasn't been revoked.
4. **Ensure Web API is Enabled:**
    * In your Firebase console, go to Project Settings > General. Make sure that the Web API is enabled.

The `bugSolution.js` file provides an example of correctly configured `firebaseConfig`.