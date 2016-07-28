#### GIT
<b>Add an repository</b>

git remote add origin yourRepository

<b>removing a cached file. </b>

git rm --cached file

Its useful, if you pushed a filer/folder, but add it later to .gitignore. With this command it won´t be pushed anymore.

<b> compare two branches for diffrences </b>

git diff branch1..branch2

<b> quit git log (e.g. git diff) </b>

q

<b> setting name </b>

git config user.name

<b> rename a branch </b>

git branch -m oldname newname

<b> checkout a local branch </b>

1. git fetch
2. git checkout remotebranch

<b> show all running processes </b>

ps

<b> kill a procress </b>

kill processnumber

<b> initialize an git branch </b>

1. don't forget: .gitignore (node_modules?, typings + .map + .js files (Typescript)?, node-debug.log?), README.markdown
2. git init
3. git add -A
4. git commit -m 'init'
5. git remote add origin yourRemoteRepo
6. git push origin master
