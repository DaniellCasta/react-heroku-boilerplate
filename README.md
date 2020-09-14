## !The most silly boilerplate

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Contains

Shows how to deploy to heroku properly, due to the lack of short information about.
Base info:
https://blog.heroku.com/deploying-react-with-zero-configuration


### How to:

1- Program your react app nicely from official boilerplate

`
npx create-react-app <your-app>
` 
or
` 
npx create-react-app@3.x $APP_NAME
` 

2- Set a local path for your project on build phase. To achieve it, modify your package.json file with the following:

`  ...
   "homepage": ".", #Or custom domain
`

3- Init your heroku settings and: 

#### `heroku create <name> --buildpack mars/create-react-app` ¡OJO!

Official way:

`heroku create -b https://github.com/mars/create-react-app-buildpack.git`

 `git remote add heroku <urlgitheroku>`
 
 `git push heroku master`

4- Do you have environment variables?

Add them via heroku env settings

#### `heroku config:set TOKEN=token123`

5- Launch your project

 `heroku open`