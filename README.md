# Getting Started with Goast

This svelte project can be used to demonstrate goast's ability to fix crashes.

## How to use this repository

1) Fork this repository if you haven't already.
2) Go to https://app.goast.ai and click the button to add a repository. Make sure to install the goast Github App in the organization where this repository exists (Probably just on your user).
3) Copy this stack trace to put into goast (Or you can click the `Use sample stack trace` button in goast)
```
Here is the fullstack trace:
+page.svelte:54 Uncaught RangeError: Maximum call stack size exceeded
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
    at createStackTraceError (+page.svelte:54:9)
```
4) Click `Generate Fix`

## About the stack trace

Goast can fix any stacktrace if it has access to the corresponding code. This means it can fix frontend or backend errors.

This example is a frontend error where a React component is referencing some state that is unexpectedly null.

## Run this sample

If you want to see the crash in action, you can run this sample yourself by installing the dependencies with `npm install` and then running `npm run start`. 
 
