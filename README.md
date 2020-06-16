## TinyPICO Echo Switch

## Attribution
This is derived from [lemariva/uPyEcho](https://github.com/lemariva/uPyEcho)
which was in turn derived from [makermusings/fauxmo](https://github.com/makermusings/fauxmo).

The how and why of this is explained in those repos.

### What is different?

* This port is TinyPICO explicit.
* It uses the MicroPython port for the TinyPICO which is different from the
    port Leamriva uses.
* It is a demo to control the onboard DotStar LED.

## How to use this?

Edit boot.py, enter your wifi SSID and Credentials.  
Sync `/src` to your TinyPico (see my Dev Workflow below).
Reset your TinyPICO in the repl `import machine` then `machine.reset()`

Once running, an Amazon Echo will be able to discover your TinyPICO. 
Your TinyPICO will have three "devices" wich can be turned on off:

* Red L.E.D.
* Blue L.E.D.
* Green L.E.D.

You can Turn On any color you want to both turn on
an unlit LED, as well as to change the color.

> Alexa, turn on Red L.E.D.

Turning off any color LED turns off the LED. It 
doesn't matter which is currently "On".

> Alexa, turn off Green L.E.D.

This also works from within the Alexa App on your phone.

## Seems like there are extra files in here
I use Micropy-CLI in my [MicroPython Dev Workflow](https://phixed.co/blog/micropython-workflow/).

## What's next?
I plan to use this example in other projects where I want control
other physical devices (appliances) using a relay wired into them. 
There's a great video on that by the [Everlanders on YouTube](https://www.youtube.com/watch?v=aS3BiYaEfiw).
Where he does this a Wemos D1 and Arduino, but the concepts will all
be the same.
