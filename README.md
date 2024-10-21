How to use Git?

----

1. create repository on GitHub
2. create local rep on your computer
3. type _git init_ in this rep.
4. ...make your work...
5. type _git add -all_ or _git add 'file name'_ to make it ready for commit command
6. make sure that all your files are 'green' by typing _git status_
7. commit your changes _git commit -m "commentary"_
8. connect local and global repositories by command _git remote add origin git@github.com:%ИМЯАККАУНТА%/first-project.git_
9. make sure that reps are connected _git remote -v_
10. and finally PUSH it, bro. First push will look like that _git push -u origin master_ then it will be just _git push_

**And dont forget about SSH certificate**, create keys on your computer by command _ssh-keygen -t ed25519 -C "электронная почта, к которой привязан ваш аккаунт на GitHub"_ and then u must connect SSH public key with GitHub.

Connection of key to GitHub u can check by command _ssh -T git@github.com_

HEAD - ur last commit, u can use it as a hash of last commit

**git log --oneline** - to view logs of ur commits in one line. 
U should make commits with comments no longer than 72 symbols.


If u wanna change last commit u should use command
**git commit --ammend --no-edit** - without changing of commit comment
**git commit --ammend -m "Updated comment of commit"** - with changing of commit comment
**--ammend WORKS ONLY WITH HEAD COMMIT**


----

Its bases of Git, bro. 
