# Github pages deploy for react projects.

<p><strong>1.</strong> Install the gh-pages package as a “dev-dependency” of the app</p>

`npm install gh-pages --save-dev`

<p><strong>2.</strong> Add homepage property to package.json file</p>

`"homepage": "http://{Github-repo-name}.github.io/"`

<p><strong>3.</strong> Deploy scripts under package.json file</p>

```
“scripts”: {
  “predeploy”: “npm run build”,
  “deploy”: “gh-pages -d build”
}
```

<p><strong>4.</strong> Add it as remote</p>

`git remote set-url origin {Github-repo-url}.git`

<p>Example:</p>

`git remote set-url origin https://github.com/supremevalidation/supremevalidation.github.io.git`

<p><strong>5.</strong> Now deploy it to GitHub Pages</p>

`npm run deploy`

<p><strong>6.</strong> Go to {your-GitHub-code-repository} -> settings -> GitHub pages section and setup source to the gh-pages branch.</p>



# Github pages deploy for angular projects.

Coming soon.
