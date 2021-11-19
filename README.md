
CRLF issues on windows:

Search all the file contains `"root": true,`

replace it with
```
"root": true,
  "rules": { "linebreak-style": ["error", "windows"] },
```


The accepted answer is great, but assuming you have Node installed, you can do this much more precisely with the node library "rimraf", which allows globbing patterns. If you use this a lot (I do), just install it globally.

```yarn global add rimraf```
then, for instance, a pattern I use constantly:

```rimraf .\**\node_modules```
or for a one-liner that let's you dodge the global install, but which takes slightly longer for the the package dynamic download:

```npx rimraf .\**\node_modules```
