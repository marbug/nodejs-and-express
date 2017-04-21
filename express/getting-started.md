# Getting Started #

## Create working directory ##

    mkdir getting-started

## Init application ##

    cd getting-started
    npm init

and input **app.js** when the following line appears:

    entry point: (index.js)

## Install Express ##

    npm install express --save

## Add application code ##

Edit **app.js** and set its code to:

    var express = require('express')
    var app = express()

    app.get('/', function (req, res) {
      res.send('Hello World!')
    })

    app.listen(3000, function () {
      console.log('Example app listening on port 3000!')
    })

## Run application ##

    node app.js

and open [http://localhost:3000/](http://localhost:3000/) in browser.

## Useful links ##

[Express Getting Started](http://expressjs.com/en/starter/installing.html)

***
|  Prev page  |  Next page                      |
| ----------- | ------------------------------: |
| [README.md](../README.md) | [Express - Generator](generator.md) |
