# basic usage
```
wpscan --url "target" --verbose
```

# enumerate vulnerable plugins, users, vulrenable themes, timthumbs
```
wpscan --url "target" --enumerate vp,u,vt,tt --follow-redirection --verbose --log target.log
```