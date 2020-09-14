## !The most silly boilerplate

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Contains

Shows how to deploy to heroku properly, due to the lack of short information about.

### How to

- Program your react app nicely from official boilerplate

`
npx create-react-app <your-app>
` 
or
` 
npx create-react-app@3.x $APP_NAME
` 

- Set a local path for your project on build phase. To achieve it, modify your package.json file with the following:

`  ...
   "homepage": ".", #Or custom domain
`

- Init your heroku settings and: 

* `heroku create <name> --buildpack mars/create-react-app` ¡OJO!
* `git remote add heroku <urlgitheroku>`
* `git push heroku master`

- Launch your project

* `heroku open`