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



