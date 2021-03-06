# Writing and Running a Node.js Program

Cloud9 IDE was built on top of the Node.js platform, and as such, you have full access to the `node` runtime. Currently, we run version v0.6.19.

In this section, we'll walk you through the creation of a simple Hello World program. To get started, you'll first need to create a (GitHub or Mercurial) project. If you need a refresher on how to do this, please refer to [Creating a New Workspace](creating_new_workspace.html).

## A Simple Node.js HTTP Server

Once you're in Cloud9, create a new file called `server.js`. Type the following code in the file:

```javascript
var http = require('http');
http.createServer(function (req, res) {
    res.writeHead(200, {'Content-Type': 'text/plain'});
    res.end('Hello World\n');
}).listen(process.env.PORT, process.env.IP);
```

This is a Node.js HTTP server. It returns a simple "Hello World" page every time you access the page. In short, you are creating an HTTP server with a callback function that is called for each request.

In the callback function, you create a response with a status code of `200` (indicating that the request was fulfilled successfully) and the message "Hello World". Finally, you specify which port and IP address the server runs on. When Cloud9 IDE runs servers, you set and retrieve the IP address and port number with the `process.env.IP` and `process.env.PORT` variables.

When you hit the ![The Run Button](./icons/runButton.png) button in the menu bar, the console will print out the following message:  
![Console run output](./images/runOutput.png)

To see your application in action, click on the link created for your project. You should see your "Hello World" application open up in a new browser tab:  
![Node.js Hello World in the Browser](./images/helloWorld.png).