# IoT Morse Code Emitter Starter Kit

In this demo, we will be getting our hands dirty the Raspberry Pi and Nodejs. We will be writing a simple program in Node.js to turn a LED on and off. Then we will extend this logic to build a simple piece of embedded system that can take a piece of string and emit its morse code.


## Materials

* 1 x Raspberry Pi (We used a Raspberry Pi 3 Model B for this demo)
* 1 x Breadboard
* 1 x 68 Ohms resistor
* 1 x LED
* 2 x Female to male wires

## Schematics

<img width="757" alt="screen shot 2019-03-08 at 12 57 45 pm" src="https://user-images.githubusercontent.com/4650739/54049573-77af5f00-41a2-11e9-84ed-63f266567f01.png">


The left end of the above circuit will be connected to Pin 9 – GND pin of pi (Left Column, 5th pin). And the right end of the above circuit will be connected to Pin 11(Left Column, 6th pin).

## Prerequesites

* Node js should be installed on your Pi - [Check out this article for tips](https://www.losant.com/blog/how-to-install-nodejs-on-raspberry-pi)
* NPM should be installed on your Pi


## Setup Your Project

Download and unpack [the project](https://github.com/devleague/ATT-Hack-IoT-Morse-Code-Starter-Kit) on your Raspberry Pi in the directory of your choice. Or alternatively checkout from source:

    git git@github.com:devleague/ATT-Hack-IoT-Morse-Code-Starter-Kit.git
    cd ATT-Hack-RPi-Sound-Sensor-Websocket-Starter-Kit

Next, inside the project, you need to install the project's various NPM dependencies:

    npm install

And you should now be ready to spin up a development build of your new project:

    npm start

Navigate to [http://localhost:3000](http://localhost:3000) in your browser of choice.

Once your breadboard is configured, you should be able to enter a message onto the form and upon submission your Pi will emit your message in morse code :tada:.

## For use on a Rasperberry Pi
Since this is the IoT, let us expose our localhost as a publicly accessible URL. We can do this using the IP Address of your Pi.

To get your Raspberry Pi's IP address. Open the terminal on your Pi and enter:

    hostname -I

![proxy duckduckgo](https://user-images.githubusercontent.com/4650739/54042197-2a75c200-418f-11e9-8399-e6f017bc8c4f.jpg)

Once you get your IP address, you should be able to access the server running on your pi by entering this in the browser of another machine:

    http:.//[YOUR_IP_ADDRESS]:3000

If you see a Morse Code website, you should be good to go!

<img width="735" alt="screen shot 2019-03-08 at 12 51 40 pm" src="https://user-images.githubusercontent.com/4650739/54049039-09b66800-41a1-11e9-9a6a-31a81dca6cc5.png">


## Contributing

1. Fork it!
2. Create your feature branch: ```git checkout -b my-new-feature```
3. Commit your changes: ```git commit -am 'Add some feature'```
4. Push to the branch: ````git push origin my-new-feature````
5. Submit a pull request :D
