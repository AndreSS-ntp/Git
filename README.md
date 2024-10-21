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

    Команда git restore --staged <file> переведёт файл из staged обратно в modified или untracked.
    Команда git reset --hard <commit hash> «откатит» историю до коммита с хешем <hash>. Более поздние коммиты потеряются!
    Команда git restore <file> «откатит» изменения в файле до последней сохранённой (в коммите или в staging) версии.

    Команда git diff сравнит последнюю закоммиченную версию файла с той, что находится в состоянии modified.
    Команда git diff --staged покажет изменения в staged-файлах относительно последних закоммиченных версий.

    Если нужно, чтобы Git игнорировал какие-то файлы, стоит составить файл .gitignore.
    Посмотреть, что игнорируется, можно с помощью команды git status --ignored.
    Сам файл .gitignore — это обычный файл в репозитории. Его тоже стоит закоммитить.
    Шаблонов много, но их легко найти в интернете вместе с примерами использования.


    git branch name-branch - creates new branch
    Команда git checkout <название_ветки> позволяет переключаться на другую ветку.
    Разные ветки в одном проекте существуют независимо. Изменения в одной не влияют на изменения в другой.
    В Git можно создать ветку и сразу же перейти в неё командой git checkout -b <название_ветки>.
    Ветка указывает на коммит, который сделан в ней последним. При этом две ветки могут ссылаться на один и тот же коммит — например, если вы только что создали ветку, но ещё не успели внести в неё коммит.
    Посмотреть и локальные, и удалённые ветки можно с помощью команды git branch -a.

git diff может сравнивать ветки по их названиям. Например, команда git diff main feature/my-feature выведет разницу между основной веткой и веткой feature/my-feature.
Git поддерживает суффикс навигации ~. 
С его помощью можно сослаться на предыдущие коммиты. 
Например, если вы находитесь в ветке main и хотите вывести разницу между тем коммитом, который был три коммита назад, и текущим, нужно выполнить git diff main~3 main.

----

Its bases of Git, bro. 
