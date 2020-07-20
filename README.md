# react-npm-publish-guide
![npm-logo](https://user-images.githubusercontent.com/8030614/87929178-b0e22980-ca8e-11ea-8aca-19bde6c8c4ef.png?s=200)
![react-logo](https://user-images.githubusercontent.com/8030614/87929180-b17ac000-ca8e-11ea-9f3e-075e8a9d0694.png?s=200)

A guide to publish a react component in NPM.


## Prerequisites
- You should have accounts at github & npm.
- Choose your package name while making sure that the name is not taken (go to [NPM](https://www.npmjs.com/) and try to search for it).
- Create a git repo with the same name as the package.


## Setup
- In your local repositories folder run: `npx create-react-library <package-name>`
(you'll have some info to fill).
- Navigate to the root folder and open 2 terminal tabs: 
In the first tab run: `npm start`, and in the second tab run: `cd example && npm start`.
- After the process is done terminate both tabs process.


## Connect to Github
From the root folder run:

`git remote add origin https://github.com/<username>/<package-name>.git`


`git push -u origin master`


## Updating the component and its demo page
- Update the component file in `src/index.js`.
- Create/update `README.md` in the root of the project.
- Update `example/src` files to show a small demo page under github pages (to run: `cd example && npm start`).
- Commit the changes.


## Deploy and publish to NPM
- Open the terminal and run: `npm login`, and enter your npm's login details.
- Delete both `package-lock.json` files in the root and under the example folder (and commit).
- Run: `npm run deploy`
- If you wish to add a public access to the package run:
`npm publish --access public`
otherwise run: `npm publish`

## *Done!!!*


### Your github page will be in:
`https://<username>.github.io/<package-name>/`

If you see a 404 page then you might need to configure it from the repo's setting.

### Tip: How to add an image of the component to a readme file:
- Go to your github page, take a screenshot of the component and save it locally.
- Go to the repository and open a new issue, drag and drop the image to the new issue, 
githb will upload and save the image and will translate it to a textual representation of it, 
copy the text and paste it anywhere in the readme file (no need to save the issue!).
