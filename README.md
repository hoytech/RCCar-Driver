# Drive an RC car with HackRF

See [this presentation](https://www.youtube.com/watch?v=1pb6B9V5UOs&t=1h27m30s) for more details.

## How to use it

You will need:

  * A [HackRF](http://greatscottgadgets.com/hackrf/)
  * A cheap remote control toy car. I used a ["coke can mini rc car"](http://www.alibaba.com/trade/search?fsb=y&IndexArea=product_en&CatId=&SearchText=coke+can+mini+rc+car) my friend ordered from China, but apparently many toys use the same protocol.

Install the pre-requisites (tested on Ubuntu 15.04):

    apt-get install libhackrf-dev
    sudo cpanm PDL SDR::Radio::HackRF Valence

Figure out the car's operating frequency with a frequency counter, GNU Radio, GQRX, whatever, then run the script:

    $ perl bin/rccar-drive 35_470_000

Use the arrow keys to drive your car around. Have fun!
