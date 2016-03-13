`heroku auth:whoami`

`cd ~/src/github/`

`mkdir nodecommand`

`heroku create nodecommand`

`curl -d '{"name": "nodecommand"}' -H X-GitHub-OTP:123456 -u davejagoda https://api.github.com/user/repos`

`git init`

`git remote add origin git@github.com:davejagoda/nodecommand.git`

`heroku git:remote -a nodecommand`

`printf '%s\n' '#emacs' '*~' '#node' 'nodemodules' > .gitignore`

`git add .gitignore`

`git commit -m 'add .gitignore'`

`git push -u origin master`

`npm init`

`npm install express --save`
