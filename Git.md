# Git Tips


## Avoid merge commit

```
git commit -m 'tempCommit' // Create a temp commit
git pull --rebase origin master // Rebase to the latest master 
// Fix any conflicts if needed and continue rebase
git rebase --continue 
// and then soft reset the head to discard the temp commit.
git reset HEAD~1
```

## Behind corporate proxy

If the certificate is untrusted you can ignore the certificate (BAD IDEA!!!)
```
git config http.sslVerify false
```

