# LaunchDarkly - Hello World using the JS client-side SDK

## Description

This is a simple test of the LaunchDarkly [JavaScript client-side SDK](https://docs.launchdarkly.com/sdk/client-side/javascript)

The index.html file contains some Javascript that renders a message based on a feature flag called "hello-world"

This example shows a feature flag called `hello-world` created with the following policy:
<img width="2043" alt="image" src="https://user-images.githubusercontent.com/17153798/198876186-43ad81aa-89e4-4377-95bb-46584ce6ff3c.png">

To test this example, load index.html from [ld.vanniekerk.com.au](https://ld.vanniekerkcom.au). Use query params for `name` and `key` to test the flag with different users. The default user `key=johndoe` should get a variation of `false`. The user `key=aaron` should get a variation of `true`, eg. https://ld.vanniekerk.com.au/?name=Aaron&key=aaron

## Steps to set this up locally

- Modify index.html
- Create a feature flag
