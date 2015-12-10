gitcrypt-test
==============

Just a test of [git-crypt](https://github.com/AGWA/git-crypt) - which was found at this [blog post](http://ebarnouflant.com/posts/3-using-git-crypt-to-transparently-encrypt-sensitive-data-in-a-git-repository).

If it works - then you shouldn't be able to read the cleartext of the included [secretfile](https://github.com/darron/gitcrypt-test/blob/master/secretfile).

Or the [sooper-sekret-passwords.yml](https://github.com/darron/gitcrypt-test/blob/master/sooper-sekret-passwords.yml) file either.

It's actually quite odd - because it appears just fine locally - and you don't see any changes to your regular flow:

```
[master]:~/Desktop/gitcrypt-test
DarronFroeseDD@: git remote add origin git@github.com:darron/gitcrypt-test.git
[master]:~/Desktop/gitcrypt-test
DarronFroeseDD@: git push -u origin master
Counting objects: 14, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (11/11), done.
Writing objects: 100% (14/14), 1.93 KiB | 0 bytes/s, done.
Total 14 (delta 0), reused 0 (delta 0)
To git@github.com:darron/gitcrypt-test.git
 * [new branch]      master -> master
Branch master set up to track remote branch master from origin.
```

But once pushed - those files are unreadable on Github.

Pretty cool.
