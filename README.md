# websocket-webgl-example

An example for how to use [device orientation](http://www.html5rocks.com/en/tutorials/device/orientation/), socket.io and express using [grunt-express](https://github.com/blai/grunt-express). The example will:

* reload the browser (when opened) using [grunt-contrib-livereload](https://github.com/gruntjs/grunt-contrib-livereload) and [grunt-regarde](https://github.com/yeoman/grunt-regarde)
* restart the server using the built-in feature of `grunt-express`, and it will do so when any of the server script is changed, or when you 'touch' the `.server` file in project root (using a `grunt-regarde` watcher setup, see `Gruntfile.js`)

The purpose of this examples is animate an image on your desktop using the orientation of your mobile phone.
 
Use Cases: Video Games, Driving Simulations, Compass

## Getting Started

1. `git clone https://github.com/azmartone/webgl-socket-example.git`
2. `npm install`
3. `grunt`


## Documentation
Replace the ip found in index.html and server.html with the server ip. If running locally, this will be your machine's network ip.

    index.html
        var socket = io.connect('http://192.168.222.101:9000');

    server.html
        var socket = io.connect('http://192.168.222.101:9000');

On your mobile device, browser to 
    http://[server]:9000

On your desktop, browse to
    http://[server]:9000/server.html

## To Do
1. Orientation metrics and animation needs to be refined.
2. Consider using acceleration rather than orientation.

## License
Copyright (c) 2014 Danny Duong  
Licensed under the MIT license.
