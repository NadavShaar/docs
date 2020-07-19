# react-npm-publish-guide
A guide to publish a react component to NPM.

### prerequisites
- You should have accounts at github & npm.
- choose your package name while making sure that the name is not taken (go to [NPM]https://www.npmjs.com/ and try to search for it).
- create a git repo with the same name as the package.

### In your local repository folder run:
`npx create-react-library <package-name>`

// open 2 terminals tabs
* First-tab: cd <package-name> && npm start
* Second-tab: cd <package-name>/example && npm start
terminate both tabs process

// From the root run:
git remote add origin https://github.com/<username>/<package-name>.git
git push -u origin master

// update with your content
update the component file in src/index.js
create/update README.md in the root of the project.
update example/src files to show a small demo page using the component, under github pages (cd example && npm start).
commit the changes.

// deploy and publish to npm
npm login (from the terminal not the browser).
delete both package-lock.json files in the root and under the example folder (and commit).
npm run deploy
** if you wish to add public access to the package run:
npm publish --access public
** otherwise run:
npm publish

Done!!!

Your gitub page will be in:
https://<username>.github.io/<package-name>/

To add an image to the readme file:
Go to your github page, take a screenshot of the component and save it locally.
Go to the repository and open a new issue, drag and drop the image to the new issue, 
githb will upload and save the image and will translate it to a textual representation of it, 
copy the text and paste it anywhere in the readme file (no need to save the issue!).
