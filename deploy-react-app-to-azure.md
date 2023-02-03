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
- In the Azure portal, type "Static Web Apps" in the search bar and click the corresponding result.
![Search for Static Web Apps](./azure-search-for-static-webapps.png)
- Click Create static web app.
![Click Create static web app](./azure-create-static-webapp.png)
- Choose the subscription you created earlier.
- For the name, type _default-react-app_. Azure will suggest a new name for the corresponding resource group.
- Make sure the plan type is _free_.
![Azure Static Webapp Options](./azure-static-webapp-options1.png)
- Set the details that correspond to your git repo. The branch will be _main_.
- Click _Review + create_.
![Azure Static Webapp Options](./azure-static-webapp-options2.png)
- Click _Create_.
![Azure Static Webapp Options](./azure-static-webapp-options3.png)
- _Click Go to resource_.
![Azure webapp created](./azure-webapp-created.png)
- In the webapp overview page, click the _Github Action runs_.
![Azure overview - Github action runs](./azure-overview-github-action-runs.png)