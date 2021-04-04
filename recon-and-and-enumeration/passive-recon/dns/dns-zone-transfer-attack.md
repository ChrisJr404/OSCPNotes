# DNS Zone Transfer Attack

## Overview

* sometimes DNS servers are misconfigured
* DNS servers contain a Zone File which It uses to replicate the map of the domain
* they should be configured so that only the replicating DNS server can access it
* if misconfigured so anyone can request the Zone File, you can receive the whole list of subdomains which is rare in the wild

## First

### figure out which DNS server a domain has

```bash
host -t ns wikipedia.com
```

```bash
host -l wikipedia.com ns1.wikipedia.com
```

### Additionally, These Tools will Help

* dnsrecon
* dnsenum

## Link to Go More in Depth

[https://security.stackexchange.com/questions/10452/dns-zone-transfer-attack](https://security.stackexchange.com/questions/10452/dns-zone-transfer-attack)

