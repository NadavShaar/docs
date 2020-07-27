# Set github-pages for react app

- Open a git repository.
- Run: `npm install gh-pages --save-dev`.
- Open `package.json' and add `homepage` set to `https://<username>.github.io/<repository-name>/`.
- Add the following scripts to `package.json`: `"predeploy": "npm run build"`, `"deploy": "gh-pages -d build"` 
  
  (`build` is the folder that contains the `bundle.js` file and it might be named dist in some cases).
- Run `git remote add origin https://github.com/<username>/<repository-name>.git` to add origin or 

  `git remote set-url origin https://github.com/<username>/<repository-name>.git` to update origin.
- Run `npm run build`.
- Run `npm run publish`.
- Commit and push repository.
- In repo's settings select `gh-pages branch` as sorce.

## *Done!!!*

### Your github page will be in:
`https://<username>.github.io/<repository-name>/`
