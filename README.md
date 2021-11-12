
CRLF issues on windows:

Search all the file contains `"root": true,`

replace it with
```
"root": true,
  "rules": { "linebreak-style": ["error", "windows"] },
```


