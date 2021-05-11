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


# Check data prediction and elapsed time in console

If everything runs smoothly, you should be able to see the logs like below in browser console.

50000079
(index):34 xprediction is 701.653202417137
(index):35 yprediction is 255.7328452199096
(index):36 clock is 34903.41000002809
(index):34 xprediction is 721.7688369396462
(index):35 yprediction is 232.72237484617136
(index):36 clock is 34969.810000038706
(index):34 xprediction is 741.1327938881816
(index):35 yprediction is 224.84369205847992
(index):36 clock is 35036.97499993723
(index):34 xprediction is 762.7510338037266
(index):35 yprediction is 214.48894141862394
(index):36 clock is 35103.57000003569
(index):34 xprediction is 706.2617460794518
(index):35 yprediction is 249.9783770482826
(index):36 clock is 35171.45000002347
(index):34 xprediction is 722.9319407746391
(index):35 yprediction is 218.26461340274523
(index):36 clock is 35238.45499998424
(index):34 xprediction is 695.3711587278825
(index):35 yprediction is 210.64145805952458
(index):36 clock is 35320.02999994438
(index):34 xprediction is 618.692215283511
(index):35 yprediction is 242.09787810305554
(index):36 clock is 35364.96000003535
(index):34 xprediction is 618.5606562404838
(index):35 yprediction is 230.40242492714654
(index):36 clock is 35415.12000001967
(index):34 xprediction is 693.6749664724019
(index):35 yprediction is 196.58739382278833
(index):36 clock is 35486.88999994192
(index):34 xprediction is 678.6457088139227
(index):35 yprediction is 204.1109953299713
(index):36 clock is 35533.46499998588
