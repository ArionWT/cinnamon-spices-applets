## What it does:

This applet keeps track of your Internet usage.

In some countries, ISPs limit the amount of data their customers can use. Passed a certain amount of bits downloaded/uploaded, you either get cut off, you pay more or your connection speed is reduced. The situation is even worse if you are using a mobile connection, especially when roaming.

## How it does it:

The vnstat daemon runs in the background and collects info about your Internet usage.

The applet detects which device you're currently using, and simply exports a graph using vnstati.

## What you need for it to work:

You need:
* To install vnstat
* To install vnstati
* To have the vnstat daemon running
* To have vnstat configured for the devices you are using.

Notes: In Linux Mint, you can simply run `apt install vnstati` and that will take care of everything for the built in devices. In other distributions it might depend on the way things are packaged but it's likely to be similar.

It is possible to add additional devices, for example a USB Mobile Internet stick. Running `man vnstat` will give some information on how to proceed but beware it is not trivial.


## Warning about use on Distributions other than Mint:

   * This Applet currently assumes the NMClient and NetworkManager libraries are available and in use as is the case in Mint versions up to 18.3 and most other current distro versions.
   * It  cannot be loaded on Fedora 27 (and possibly future versions of Linux Mint or other distros) due to the move from NMClient and NetworkManager libraries to NM.
   * Attempting to add this applet on Fedora 27 may cause Cinnamon to continually crash (issue #1647).

### Support

The original author of this Applet was Clem. More recently it has been supported by @pdcurtis who occasionally checks the comments on the [Cinnamon Spices Web Site](http://cinnamon-spices.linuxmint.com/applets/view/31), however that does not automatically notify him so if you want a rapid response please also note that mentioning @pdcurtis in any conversation on github will cause it to be emailed to him.

