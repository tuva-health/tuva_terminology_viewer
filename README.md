# Tuva Terminology Viewer

## Instructions to deploy this to github pages.

### Install the `gh-pages` package.

`npm install --save-dev gh-pages`

### Update `package.json`

Add the following configurations to your package.json file:

- Set the homepage field to point to your GitHub Pages URL. Replace username with your GitHub username and repo-name with your repository name:
`"homepage": "https://username.github.io/repo-name"`

- Add deployment scripts under the scripts section:
`"scripts": {
  "predeploy": "npm run build",
  "deploy": "gh-pages -d build"
}`

- Deploy the App
Run the deployment command:
`npm run deploy`

Enable GitHub Pages in Repository Settings  
- Go to your repository on GitHub (e.g., https://github.com/username/repo-name).
- Click on Settings.
- Ensure your repo is public, otherwise you cannot share this via pages.
- Scroll to the Pages section.
- Under Source, select the gh-pages branch and set the folder to / (root).
- Click Save.
