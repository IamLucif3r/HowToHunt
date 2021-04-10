## Hostile Subdomain Takeover Methodology

### What is Hostile Subdomain Takeover ?
One of the subdomains of the scanned domain is pointing to an external service but the external service account was cancelled or has expired. Because the account is not in use anymore, an attacker can claim this account and takeover your subdomain. The attacker can use this subdomain for phishing or to spread malware

### Tool
You can use [HostileSubBruteforcer](https://github.com/nahamsec/HostileSubBruteforcer), for checking if any subdomain can be taken over.
This app will bruteforce for exisiting subdomains and provide the following information:
 - IP address
 - Host
 - if the 3rd party host has been properly setup. (for example if site.example.com is poiting to a nonexisiting Heroku subdomain, it'll alert you) -> Currently only works with AWS, Github, Heroku, shopify, tumblr and squarespace.


### Approach
1. Find a subdomain pointing to a third-party using HostileSubBruteforcer {is an alias of x.com}
2. Make sure their service is inactive / expired / cancelled
3. Go to the third-party website, and register as client. When you have to choose the subdomain, enter the subdomain you are testing.

