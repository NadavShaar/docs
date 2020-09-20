# Deploy a node app to Heroku
- Open `package.json` and add the engines property with your node version.
`"engines": {
    "node": "10.x"
}`
- Push all changes to git.
- Run `heroku login`.
- Run `heroku create <project-name>`.
- Run `git push heroku master`.

## *Done!!!*