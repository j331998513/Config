``
git config -l

// to check if core.autocrlf=false
// if so then:

git config --add core.autocrlf true

//otherwise 
git rm --cached -r .
git reset --hard

```
