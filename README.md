# tem blog@sunsin.shop
- Our team's technology blog inherits the spirit of Admiral Yi Sun-sin of Joseon
  
<img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSzdREgTNnlP6Bo7iXtMIhUHOygOEk1c0nYiQ&s" alt="team sunsin" style="width:600px;"/>

### Connecting
- PRD - https://team.sunsin.shop, https://wminhyuk.github.io/
- STG - https://team-sunsin.web.app
- DEV - 
- LOCAL - https://localhost8000

### Contribute guide
- Anyone can do it's possible. Let's send the PR first and make it a better team by joining.

0. created based on [vuepress](https://v2.vuepress.vuejs.org/)
1. git clone git@github.com:sunsin-shop/sunsin.github.io.git
2. edit with [vscode](https://code.visualstudio.com/) OR VIM
3. install
``` bash
https://github.com/nvm-sh/nvm
https://pnpm.io/ko/
```
4. run - development environment [install pnpm](https://pnpm.io/installation)
- connecting to localhost 8080
- node.js install if you have get error 'ELIFECYCLE Command failed'
```
$ nvm install --lts
$ nvm ls
$ nvm use v22.13.0
$ node -v
v22.13.0
$ pnpm install
$ pnpm docs:dev
```

### build & deploy
1. STG
- [x] 배포전 작업 파일은 모두 커밋!
- [install firebase](https://v2.vuepress.vuejs.org/guide/deployment.html#google-firebase)

``` bash
$ sh deploy-stg.sh

=== Deploying to 'oss-cashmallow'...

i  deploying hosting
i  hosting[oss-cashmallow]: beginning deploy...
i  hosting[oss-cashmallow]: found 43 files in ./docs
✔  hosting[oss-cashmallow]: file upload complete
i  hosting[oss-cashmallow]: finalizing version...
✔  hosting[oss-cashmallow]: version finalized
i  hosting[oss-cashmallow]: releasing new version...
✔  hosting[oss-cashmallow]: release complete

✔  Deploy complete!

Project Console: https://console.firebase.google.com/project/oss-cashmallow/overview
Hosting URL: https://oss-cashmallow.web.app
╞╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╡╞╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╡
다음 항목을 제거할 예정입니다:
  docs/assets/app-a5e3f83c.js         docs/assets/index.html-77e713f0.js  docs/team/how2pr/
  docs/assets/index.html-6e725bfb.js  docs/assets/index.html-a3f200a8.js
*** 명령 ***
    1: clean                2: filter by pattern    3: select by numbers    4: ask each             5: quit
    6: help
무엇을 할까요> 1
docs/assets/app-a5e3f83c.js 제거
docs/assets/index.html-6e725bfb.js 제거
docs/assets/index.html-77e713f0.js 제거
docs/assets/index.html-a3f200a8.js 제거
docs/team/how2pr/ 제거
╞╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╡╞╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╪╡
STG DEPLOY OK!
https://oss-cashmallow.web.app
```

2. PRD
- github pages -> docs
- pnpm docs:build
- git push * PR merge

<img src="https://user-images.githubusercontent.com/120996497/212484360-1b212db0-5a5c-449f-8cc2-35de2126bd66.png" alt="cashmallow" style="width:600px;"/>
<img src="https://oss-cashmallow.github.io/images/hero.png" alt="cashmallow" style="width:200px;"/>
