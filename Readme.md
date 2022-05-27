# httpserver

httpserver is a Go program that provides you with the Download files from httpserver.

## Prerequisites

Install go and curl before run 

and

put file (test.txt) on C:\inetpub\wwwroot\new 



## Usage

```
##Server
...>go run httpserver1.go new
Server Running...
Listening on localhost:9980
Waiting for client...
A new client connected
Read a new line from connection: 'GET /test.txt HTTP/1.1'
line GET /test.txt HTTP/1.1
Got new 'GET' request for /test.txt
Read a new line from connection: 'Host: 127.0.0.1:9980'
Decoded new header line with value 'Host' and value '127.0.0.1:9980'
Read a new line from connection: 'User-Agent: curl/7.79.1'
Decoded new header line with value 'User-Agent' and value 'curl/7.79.1'
Read a new line from connection: 'Accept: */*'
Decoded new header line with value 'Accept' and value '*/*'
Read a new line from connection: ''
Hi
Downloaded /test.txt
Sent response with status code: 200

##Client

...>curl http://127.0.0.1:9980/test.txt
File Download Successfully

```

