
CRLF issues on windows:

Search all the file contains `"root": true,`

replace it with
```
"root": true,
  "rules": { "linebreak-style": ["error", "windows"] },
```


Setup for windows environment
```
1. npm install dotenv@^8.2.0
2. yarn install
3. yarn webpack:dlls:windows

if you want to delete node_modules in case any issues occured

npx npkill
then repeat above 1-2-3 process

```
