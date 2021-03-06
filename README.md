# VAULT 
swiss army knife for hackers

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/740204dd950c4e49841c94f2c32af78a)](https://app.codacy.com/app/abhisharma404/vault_scanner?utm_source=github.com&utm_medium=referral&utm_content=abhisharma404/vault_scanner&utm_campaign=Badge_Grade_Dashboard)
[![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/abhisharma404/vault_scanner) 
[![Join the chat at https://gitter.im/vault_scanner/kwoc](https://badges.gitter.im/vault_scanner/Lobby.svg)](https://gitter.im/vault_scanner/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) ![Python](https://img.shields.io/badge/python-%3E%3D3-brightgreen.svg)
![version](https://img.shields.io/badge/version-0.1.0-yellow.svg)

* #### Scan website for the following vulnerabilities
- [x] XSS
- [x] LFI
- [ ] RFI
- [ ] SQLi

* #### Scan for common header errors
- [x] Clickjacking
- [ ] jQuery version checking
- [x] Insecure cookie flags
- [ ] Session fixation through cookie injection
- [x] Testing HTTP methods
- [x] Insecure headers
- [ ] Brute force login through Authorization headers

* #### Collecting data
- [x] Port scanning : ACK, FIN, NULL, XMAS
- [x] IP scanning : Ping Sweep
- [x] SSL Scanner
- [x] URL Fuzzer
- [x] Header/banner grabbing
- [x] Find comments in source code
- [x] WHOIS Lookup
- [x] Google Dork
- [ ] OS Scan
- [ ] Error handler checker
- [ ] Admin panel finder
- [ ] CMS Detection
- [ ] Detect Honeypots
- [ ] Detect DDoS attack
- [ ] Open redirect vulnerability testing

* #### Crawling
- [ ] Crawl a website and collect all the links
- [ ] Crawl and scrape the website for images

* #### Attacks
- [x] DDoS Attack
- [ ] ARP Spoofer
- [ ] DNS Spoofer
- [ ] De-authentication attack
- [ ] Shellsock

* #### Utilities
- [ ] Generate customized backdoor
- [ ] Hash scanner
- [ ] Data monitoring
- [ ] Keylogger
- [ ] SSH Tunelling 
- [ ] Generate sitemap
- [ ] Mac address changer
- [ ] Trace route

# Getting Started

Steps to setup :

1. `git clone <your-fork-url>`
2. `cd vault_scanner`
3. `sudo apt-get install python3-pip`
4. `sudo pip3 install virtualenv`
5. `virtualenv venv`
6. `source venv/bin/activate`
7. `pip3 install -r requirements.txt`

Starting Vault :

1. `cd vault_scanner/src`
2. `python3 vault.py`

# Usage

```
usage: vault.py [-h] [-u URL] [-p PORT] [-sp START_PORT] [-ep END_PORT] [-ssl]
                [-info] [-comment] [-fuzz] [-ip IP] [-t THREADS]
                [-source_port SOURCE_PORT] [-fin] [-null] [-ack] [-xmas] [-c]
                [-xss] [-this] [-ping_sweep] [-ip_start_range IP_START_RANGE]
                [-ip_end_range IP_END_RANGE] [-lfi] [-whois] [-o OUTPUT]
                [-d DORK]

optional arguments:
  -h, --help            show this help message and exit
  -u URL, --url URL     URL for scanning
  -p PORT, --port PORT  Single port for scanning
  -d DORK,--dork DORK   Performs Google Dorking
  -sp START_PORT, --start_port START_PORT
                        Start port for scanning
  -ep END_PORT, --end_port END_PORT
                        End port for scanning
  -ssl                  perform SSL scan
  -info                 Gather information
  -comment              Finding comments
  -fuzz                 Fuzzing URL
  -ip IP, --ip IP       IP address for port scanning
  -t THREADS, --threads THREADS
                        Number of threads to use
  -source_port SOURCE_PORT
                        Source port for sending packets
  -fin                  Perform FIN Scan
  -null                 Perform NULL Scan
  -ack                  Perform TCP ACK Scan
  -xmas                 Perform XMAS Scan
  -c, --crawl           Crawl and collect all the links
  -xss                  Scan for XSS vulnerabilities
  -this                 Only scan the given URL, do not crawl
  -ping_sweep           ICMP ECHO request
  -ip_start_range IP_START_RANGE
                        Start range for scanning IP
  -ip_end_range IP_END_RANGE
                        End range for scanning IP
  -lfi                  Scan for LFI vulnerabilities
  -whois                perform a whois lookup of a given IP
  -o OUTPUT, --output OUTPUT
                        Output all data
```

Example Usage :

`python3 vault.py -u 'http://url' -info -comment -ssl -fuzz`

# Screenshot

![](logo/Initial_Setup.png)

### This project is currently a part of IIT KWoC 2018.
