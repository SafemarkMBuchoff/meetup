### The instructions below are for Windows, but the steps for Mac or Linux are similar
- Create a new Azure account
- Create a new subscription within that Azure account (TODO: flush these steps out)
-  On your local computer, install NodeJS
```
winget install -e --id OpenJS.NodeJS
```
- Create a barebones react app
```
npx create-react-app default-react-app
```
- Test it out
```
cd default-react-app
npm start
```
After a few seconds, a browser tab should open and you should see a barebones react app.
![Barebones React app](./barebones-react-app.png)

- Create a repository on github
![New repo on GitHub](./github-new-repo-button.png)
![Name of the repo](./github-new-repo-name.png)
![Name of the repo](./github-new-repo-confirm.png)

- Add your react app to your new repo by pasting these commands into the command line:
![Add react app to repo](./add-react-app-to-repo.png)
```
git remote add origin YOUR_REPO_URL
git branch -M main
git push -u origin main
```
