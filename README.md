# LaunchDarkly - Hello World using the JS client-side SDK

## Description

This is a simple test of the LaunchDarkly [JavaScript client-side SDK](https://docs.launchdarkly.com/sdk/client-side/javascript)

The index.html file contains some Javascript that renders a message based on a feature flag called "hello-world"

This example shows a feature flag called `hello-world` created with the following policy:
<img width="2043" alt="image" src="https://user-images.githubusercontent.com/17153798/198876186-43ad81aa-89e4-4377-95bb-46584ce6ff3c.png">

To test this example, load index.html from [ld.vanniekerk.com.au](https://ld.vanniekerk.com.au). Use query params for `name` and `key` to test the flag with different users. The default user `key=johndoe` should get a variation of `false`. The user `key=aaron` should get a variation of `true`, eg. https://ld.vanniekerk.com.au/?name=Aaron&key=aaron

## Steps to set this up locally

- (Optional) [Create a new LaunchDarkly account](https://launchdarkly.com/start-trial/)
- Create a Project (take note of the `Client-side ID` for the applicable environment)
- Create a new feature flag (remember to set `SDKs using Client-side ID`)
<img width="637" alt="image" src="https://user-images.githubusercontent.com/17153798/198876948-a5bd3256-e436-4f65-8a76-b70225381a3c.png">
- Create a Targeting policy (you may have no users at this point if you're using a new account)
<img width="2049" alt="image" src="https://user-images.githubusercontent.com/17153798/198877104-ca8900ba-1796-45aa-99a1-f90ca8743578.png">
- Download index.html
- Replace the Client-side ID in LDClient.initialize() with your own
- Open index.html in your browser and start testing!
