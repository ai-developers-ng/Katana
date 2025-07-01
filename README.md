# Katana-ds (dork scanner) (Stable) 
[![Github All Releases](https://img.shields.io/badge/Katana--ds-version%201.5.3-red)]()
[![Github All Releases](https://img.shields.io/badge/support-python%203.7%2F3.8%20%2B-brightgreen)]()
[![Github All Releases](https://img.shields.io/badge/platform-windows%20%7C%20linux-lightgrey)]()
[![Github All Releases](https://img.shields.io/twitter/follow/TebbaaX)]()

Katana-ds (ds for dork_scanner) is a simple python tool that automates Google Hacking/Dorking and supports Tor.
It becomes a more powerful in combination with [GHDB](https://www.exploit-db.com/google-hacking-database)

**Note 25/09/2021** : This Repo is New but the script it self is old back when google dorking was something, i wrote this script back in Highschool during the process of learning how to "scrape" using python and in order to get to use on bs4 and other Python packages and i learned alot of things along, still there's alot of people who use this script... Thanks for 500 ⭐... Oh and OSINT too.


**Note 01/07/2025** : This is a Google Dorking tool I originally wrote around 8 years ago, back when I was just starting to explore scripting, automation, and basic OSINT. I only uploaded it to GitHub a few years later — mostly for fun — not expecting it to gain much attention.

- Fast-forward, and somehow it’s sitting at 1.2k stars. Wild!

Looking back, the code is… let’s say, “educational.” But I’ve decided to leave it up because:

 - It’s a fun reminder of where I started,

- Some folks still find it useful (or nostalgic),

- And honestly? It’s part of the journey.

If you’re just browsing, enjoy the blast from the past! 

I worked on another tool that was inspired by [Tomnomnom's wwww from Nahamcon on how to make your own wordlist](https://tomnomnom.com/talks/wwwww.pdf) if you are into web security and more.




![Alt text](https://github.com/TebbaaX/imgs/blob/master/img1.jpg)

## Installation :

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install requirements

```bash
cd Katana
python3 -m pip install -r requirements.txt
python3 kds.py
```

### Tested on Windows [ConEmu](https://conemu.github.io/)  [![Github All Releases](https://conemu.github.io/img/logo.png)]()

## Usage :

```bash
cd Katana
python3 kds.py -h (for help)
Options :
-g :for google mode
-s :for scada mode
-t :for tor mode
-p :for proxy mode
```

## What's new in Katana-ds V1.5.3 :

- No need to set the TLD in google Mode
- No need to set the TLD in Scada Mode
- More Scada Results (after adding More dorks)
- Partially solved the HTTP Errors
- Proxy Mode will display 100 proxy server each time

## Google Mode : (supported by python 3.7 and 3.8)
Google mode gives you 1 input to set the "Dork"


## Scada Mode : (supported by python 3.7 and 3.8)

Scada mode search in google for online Scada devices

-!> this is just an example actually it shows a lot of results



Example of [Allen-Bradley](https://ab.rockwellautomation.com/lang-selection.html) PLC dashboard found using Scada Mode


## Tor Mode : (supported by python 3.7 and 3.8)

[![Github All Releases](http://icons.iconarchive.com/icons/blackvariant/button-ui-requests-8/256/Tor-icon.png)]()

Tor mode gives you 1 input which is the search query but before you should have tor proxy running on port 9050 this time there is no IP blocking the script search in 3 tor search engines Phobos, Tor66 and Tordex (more will be added)

-!> this is just an example actually it shows a lot of results



![Alt text](http://icons.iconarchive.com/icons/graphicrating/koloria/32/Warning-2-icon.png)

## What if :

- The script print 'HTTP Error 429 too many requests' :
**change the TLD**
- The script print 'urllib.error.URLError Errno 1104' :
**check if the TLD is true**
- Changing the TLD doesn't work : (2 solutions)
**1-change your ip by disconnecting and reconnecting again or use a good vpn**
**2-Delete the .google-cookie file in Katana Directory**
- Tor mode show 'Failed to establish a new connection' :
**make sure that tor proxy up and running on port 9050**

## Proxy Mode : (supported by python 3.7 only)

Proxy mode find proxy servers and print them it will print 100 Different Proxy server Each time


## Please feel free to open ISSUES or contact me on [twitter](https://twitter.com/TebbaaX) 

## License

[MIT](https://github.com/TebbaaX/Katana/blob/master/LICENSE.txt)
