# snapwat?

**Work in progress...**

sna**pwa**t is a demo to showcase progressive web app capabilities.

The idea of the app is to let you doodle and add emojis etc. on top of photos and videos.
It may or may not have taken some inspiration from certain social apps' "Stories" features ;-D

<img src="docs/first-version.jpg?raw=true" alt="First version" width="300px"/> 

This demo is intended to be as lightweight as possible. However, it would be a shame to avoid
all modern tooling and lose out on the latest syntax and JS bundling. So, I'm using 
[Babel](https://babeljs.io/) to transpile the ES2015 syntax and [rollup](http://rollupjs.org) 
for module loading.

The [WebRTC adapter](https://github.com/webrtc/adapter) is used to polyfill the latest 
MediaDevices promise-based API.

## Local development

As usual, the best place to begin is:

```npm install```

Then to transpile and combine the JavaScript:

```npm run build```

(This just runs `rollup -c > build/bundle.js`).

To run the app, you can use any static web server. I just use `python -m SimpleHTTPServer`.

To watch for changes (in a separate terminal):

```npm run watch```

(This just uses `watch` to rebuild the JS when a change is detected in the src directory).
