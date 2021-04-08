## Run a simple HTTPs server to host this static page

Follow the readme file in this repo to install a simple web server.
https://github.com/http-party/http-server

Then just run it:
```
http-server -S -C cert.pem
```

A great WebGazer video tutorial: 
https://www.youtube.com/watch?v=NRLlRh2apA8

To allow Chrome to access local self-signed webpage, navigate to
```
chrome://flags/#unsafely-treat-insecure-origin-as-secure
```