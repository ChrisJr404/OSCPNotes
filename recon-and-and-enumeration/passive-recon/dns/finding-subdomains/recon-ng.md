# recon-ng

## Overview

* full-featured web recon framework written in Python
* same basic structure as Metasploit

## Find Subdomains

```bash
recon-ng
use use recon/domains-host/
show options #shows vast amount of alternatives
set source website.com #all subdomains will be saved in "hosts"
show hosts #which you can use with
```

## Resolve IPs of Subdomains if Not Automatic

```bash
use recon/hosts-hosts/resolve
run #resolve all hosts in the host file
```

