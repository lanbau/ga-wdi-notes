#Setup Account on Heroku
- Create New App
- Connect to GitHub
- Travis CI , auto enable
-  Review Apps - develop new feature on separate domain -> pull request to main domain
- create new review apps for new pull requests automatically

#install heroku toolbelt
- cd to folder
- git remote add heroku git@heroku.com:lanbau-tictactoe.git
- git remote -v
- heroku buildpacks:set heroku/nodejs

#Install server
- npm install --save http-server
- http-server
- http-server Tictactoe
- npm start


- add this to package.json - "start": "npm run build && http-server game",
- "clean": "rm -rf dist",
- "build": "npm run clean && mkdir dist && npm run build-html && npm run build-css && npm run build-js",
- "build-html": "cp index.html dist/index.html",
- "build-css":"cp app.css dist/app.css",
- "build-js": "browserify app.js --outfile dist/app.dist.js --transform babelify"

- check with travisjs
- push to new branch(feature)
- deploy via feature
