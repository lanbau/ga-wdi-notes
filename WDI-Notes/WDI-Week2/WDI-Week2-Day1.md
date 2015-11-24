#Port over to Safari

#Create Package JSON
- npm init
- cat package.json
- npm install babelify browserify babel-preset-stage-0 babel-preset-es2015 --save
- browserify app.js --outfile app.dist.js --transform babelify

#EDIT Node Modules
-  PATH="./node_modules/.bin:/Library/Frameworks/Python.framework/Versions/3.4/bin:${PATH}"

#Ignore redundant files
add .gitgnore
#add to Package.json
"build": "browserify app.js --outfile app.dist.js --transform babelify"

#Everytime you make changes to the file do this to convert file
npm run build

#Run Standard
npm install standard
standard
change packagejson -> "test": "standard"

codeship.com
travis-ci.org
