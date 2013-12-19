skynetjs
========

Skynet Javascript for making client-side IoT development easier

Note: There are three ways listed in the HTML example:

1. The first option is used when you know the UUID and token of the device or node being connected to Skynet

```
var skynetConfig = {
  "uuid": "0d3a53a0-2a0b-11e3-b09c-ff4de847b2cc",
  "token": "qirqglm6yb1vpldixflopnux4phtcsor"
}    
skynet(skynetConfig, function (e, socket) {
````

2. If you would like for Skynet to automatically register a new UUID and token for you.

```
skynet(function (e, skynet) {
```

3. Similar to option two, Skynet will automatically register your device/node but you can pass additional JSON elements to your device description. There are no reserved element names.

```
skynet({appName:'chris'}, function (e, skynet) {
```
