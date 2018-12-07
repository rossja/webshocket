# WebSHocket

A Golang based webshell that uses websockets for the command channel

## Overview

This tool is heavily based on the [gorilla command example](https://github.com/gorilla/websocket/tree/master/examples/command).

I've made some minor modifications that: 

1. hard-code `/bin/sh` as the command to bind to the websocket
2. support running the server on a user-specified port
3. embed the html content as b64 encoded string rather than using an external file 
  - (this is, arguably, more useful for red-teaming scenarios)
  
# Binaries

If you don't care to compile this yourself, I release the program as binaries for Mac, Linux, and Windows on x86, amd64, arm, and arm64. Just grab them from the [releases link](https://github.com/rossja/webshocket/releases)
