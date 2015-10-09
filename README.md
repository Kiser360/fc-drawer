# fc-drawer
This is a webapp for drawing on an 64 LED array in 8x8 configuration controlled with a fadecandy controller.  To visit the app head here: http://kiser360.github.io/fc-server/dist

Control the array by first connecting to a fadeCandy Server, by default it will attempt to connect to localhost:7890 or you can enter your server's hostname in the settings menu.  You can also use the app without a fadecandy server or LED array.  To start select a color by dragging the FAB in the bottom right to the color of your choice, whether that be from the preset colors or your own color from the gadient that appears to the left.  Once you have a color get started drawing!

## How to start developing

####Take care of some dependencies!
1. Install Node: https://nodejs.org
2. 
```
$ npm install -g gulp && npm install -g bower && npm install && bower install
```
####Serve locally
```
$ gulp serve
```

####Build for Deployment
```
$ gulp build
```
All files will be minimized/vulcanized/consolidated in the dist folder

####Run some tests
```
gulp test:local
```
All tests are located in app/test

####Credits
Built using Polymer: https://www.polymer-project.org

Tested with WebComponentTester (runner) and Mocha, Chai, Sinon

Communication with WebSockets via OPC protocol: http://openpixelcontrol.org/

Suggested Browser: Chrome or Firefox; untested in IE, Opera, Safari etc.

LEDs controlled by FadeCandy: https://www.adafruit.com/products/1689
