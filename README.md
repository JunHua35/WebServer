# WebServer

## This is a rudimentary HTTP server created based on a TCP server and some parsing logic.

Note: For my reference only, most of the stuff in here was copy pasted from the website 

To execute:
1) Download WebServer.js or WebServerLite.js
2) Run the file from your command line with `node *filename*`.
3) In another terminal use cURL to make a simple request to your server: `curl -v localhost:3000/some/url` \
   It should show something like this: 
> Received chunk:\
GET /some/url HTTP/1.1 \
Host: localhost:3000 \
User-Agent: curl/7.54.0 \
Accept: */*
5) Alternatively you can make a POST request with some data: `curl -v -X POST -d'hello=world' localhost:3000/some/url` \
   It should show something like this:
> Received chunk: \
POST /some/url HTTP/1.1 \
Host: localhost:3000 \
User-Agent: curl/7.54.0 \
Accept: */* \
Content-Length: 11 \
Content-Type: application/x-www-form-urlencoded \
hello=world
6) That's it! You can now see how HTTP requests and responses work.
   
Adapted from this [website](https://www.codementor.io/@ziad-saab/let-s-code-a-web-server-from-scratch-with-nodejs-streams-h4uc9utji) \
Also credits to [CodeCrafters](https://github.com/codecrafters-io/build-your-own-x)
