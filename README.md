# test-project

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For detailed explanation on how things work, checkout the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

# Vue-project

``` bash
# how to set up the development environment
# install the Vue Command Line Interface globally
npm install -g vue-cli

# initialize webpack and name your project (ex: project-name) 
npm init webpack project-name

# answer all of the following questions (feel free to keep defaults)
Project name: project-name
Project description: A Vue.js project
Author: Your Name
Vue build: standalone
Install vue-router? No
Use ESLint to lint your code? No
Setup unit test with Karma + Mocha? No
Setup e2e tests with Nightwatch? No

# follow their next steps to get started:
cd project-name
npm install

# how to run the development server
npm run dev

# project will be deployed on localhost:8080
# dependencies can be located in the newly created node_modules folder
# make any customizations to the projects that you desire
# be sure to use debugging tools (like the Sources tab in the Chrome development tools) to test and debug your code in the local environment

# how to build the code for deployment on Github
# configure webpack to build code into /docs folder instead of default /dist folder
open config/index.html in your code editor
change all instances of dist to docs
change the path from root ('/') to none ('')

build: {
    ...
    index: path.resolve(__dirname, '../docs/index.html'),
    assetsRoot: path.resolve(__dirname, '../docs'),
    ...
    assetsPublicPath: '',
    ...
}

save changes

# run the build command again to create the docs folder
npm run build
# how to deploy the site
create a new repo in Github 
do not create a new README or LICENSE files
follow their directions to create the new repository from files on the command line (instead of 'git add README.md', use 'git add -A' to add all of the files in your folder)
check your Github to make sure all folders have published
click "Settings" and find section on GitHub Pages
change Source to master branch /docs folder
click Save
cilck on the website provided to view your Vue app webpage!