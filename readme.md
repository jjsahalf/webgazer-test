# Do these things to have everything set up

## Run this script in terminal.
./run-this.sh

## To allow Chrome to access local self-signed webpage, navigate to
```
chrome://flags/#unsafely-treat-insecure-origin-as-secure
```

# The script does the following things for you.

## Install homebrew if you haven't

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

or go to homebrew homepage to learn more.

## Install openssl if you haven't

brew install openssl

## Install a simple http server if you haven't

brew install http-server

or 

follow the readme file in this repo to install a simple web server.
https://github.com/http-party/http-server

## Create a certificate for http TLS session

openssl req -newkey rsa:2048 -new -nodes -x509 -days 3650 -keyout key.pem -out cert.pem

## Run a simple HTTPs server to host this static page

Run the command below in the terminal under the path of your static web page.
```
http-server -S -C cert.pem
```

A great WebGazer video tutorial: 
https://www.youtube.com/watch?v=NRLlRh2apA8

