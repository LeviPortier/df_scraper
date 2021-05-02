# Explanation
requirements.txt contains the python requirements
crawlers contain the notebooks with crawlers for the four different marketplaces
data contains the scraped data
scraper.ipynb contains the scraping of the crawled data
]
In each ipynb the code is clearly explained using comments


# Setup 
This code runs in linux ubuntu 20.04

### Download Geckodriver
Install geckodriver from https://github.com/mozilla/geckodriver/releases/
make sure the geckodriver bin file is located in ```/usr/bin```

### Configuring TOR

Download tor
```bash
$ sudo apt install tor
```
and download the tor browser bundle via their website

#### testing configuration

```bash 
from tbselenium.tbdriver import TorBrowserDriver
with TorBrowserDriver("/path/to/TorBrowserBundle/") as driver:
    driver.get('https://check.torproject.org')
```
```/path/to/TorBrowserBundle``` should look something like this ```home/usr/tor-browser_en-US/```

the folder contains a folder Browser, which contains the firefox binary.

    



