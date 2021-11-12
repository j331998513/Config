```
git config -l

// to check if core.autocrlf=false
// if so then:

git rm --cached -r .
git reset --hard

//otherwise 
git config --add core.autocrlf false
git rm --cached -r .
git reset --hard

```
