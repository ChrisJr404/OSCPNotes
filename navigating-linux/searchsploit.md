# searchsploit

## Show Exploit-DB Link Instead of Local Path

```text
searchsploit example search -w
```

## Search Exploit Title

```text
searchsploit example search -t
```

## Show Only the Link of Results

```text
searchsploit example search -w -t | grep http | cut -f 2 -d "|"
```

## Download All RAW Files of Results

```text
for e in $(searchsploit example search -w -t | grep http | cut -f 2 -d "|"); do exp=$(echo $e | cut -d "/" -f 5) && url=$(echo $e | sed 's/exploits/raw/') && wget -q --no-check-certificate $url -O $exp; done
```

