# chai aur backend series

This is a video series on backend with javascript
- [Model link](https://app.eraser.io/workspace/YtPqZ1VogxGy1jzIDkzj?origin=share)

# step-1
# How to create node js backend ?
# npm init

step-2
create src folder

step-3
inside src create below file
touch app.js constants.js index.js

step-4
## If you want to import  something using import keyword then add 'module' in package.json
# "type": "module"

## How to auto restart server after file save
# using Nodemon 
# npm i -D nodemon
# "dev": "nodemon src/index.js"

step-5
create below folder
mkdir controllers, db, middlewares, models, routes, utils

step-6 (optional)
install prettier
-D use for developer
npm i -D prettier


step-7
install below packages
npm i  express mongoose dotenv

step-8
-> connect db (all code are in the db/index.js)
-> import in index.js(all code are in index.js)
-> we are imprt (import dotenv from 'dotenv') so we change in package.json
    ->"dev": "nodemon -r dotenv/config  src/index.js"