# Making your own Nitroless repo

 If you'd like to make your own collection of emotes for Nitroless, make a fork of this repo by pressing `Use this template` and follow the steps below!

 1. You'll want to have Node JS installed to run the automated script to generate the manifest JSON and resize emotes automatically. You can download it [here](https://nodejs.org/en/download/).

 2. Edit repoData.js with the appropriate details for your repo. For example:
 ```js
//Add Name of your Repo here
exports.name = `Example Repo`;
//Add Name and Type of Image Icon you want to use here
exports.icon = 'CoolIcon.png';
//Add the folder name where all your emotes are saved
exports.pathName = 'emotes';
//Add your name here, or remove the line if you don't need your name displayed under the repo's title in our clients
exports.author = 'Joe';
```

3. Add all of your emotes to the folder you're using. Make sure they're all PNGs, JPGs or GIFs. 

4. Run `npm i` in the root directory of the repo to install the required dependencies.

5. Run `npm run start` to generate the manifest JSON and resize all emotes correctly. 

6. Now host this repo to a web server or use GitHub Pages to host it. GitHub Pages help is available [here](https://pages.github.com/).

> If using GitHub Pages, you might want to edit this ReadMe to include a link to your repo with this URL Scheme `nitroless://add-repository?url=https://epic.nitroless.repo/`

## Pushing Updates

Pushing updates is easy! Just rerun `npm run start` and push the changes to your repo. The manifest will be updated automatically to add new emotes and remove deleted ones.
