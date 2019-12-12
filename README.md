# AppsScript-HTML-Starter
<h2>Overview</h2>

Create and Host a website with Apps Script. Work locally using your favorite IDE. Use HTML, CSS, and JavaScript to design your pages. Use `clasp` to push your code files to Google Drive and to deploy your site to Google Cloud Platform.

This project uses npm to install clasp. The clasp CLI lets you work on Apps Scripts locally and then push and deploy changes from your Terminal or IDE.

<h2>Instructions</h2>

<h3>Clone the project and install clasp</h3>

```
git clone git@github.com:ChaddPortwine/AppsScript-HTML-Starter
cd AppsScript-HTML-Starter
npm install
```
<h3>Give clasp permission to use your account</h3>

Run `clasp login`. This will open a browser where you must login and click through to grant clasp access to a few Google services. Once complete, return to your terminal or IDE.

<h3>Enable the Google Apps Script API</h3>
Open your Apps Script user settings.

https://script.google.com/home/usersettings

Turn on Google Apps Script API and return to your terminal or IDE.

<h3>Create a new Apps Script Web App</h3>

Use `clasp` to create a new blank Apps Script project. Set the type, title, and directory.
```
clasp create --type webapp --title "AppsScript-HTML-Starter" --rootDir ./
```

<h3>Push your local files to Google Drive.</h3>

Run `clasp push` to send your changes to Google Drive (aka script.google.com).

```
clasp push
└─ Code.gs
└─ appsscript.json
└─ index.html
Pushed 3 files.
```
<h3>Deploy your app to Google Cloud Platform</h3>

Run `clasp deploy` to deploy your app to GCP. Within your project, a new version is created and then published.

```
clasp deploy
Created version 1.
- AKf...LEQ @1.
```
<h3>Open the Web Page</h3>

Run `clasp open --webapp` and select a deployment to open your web page in a browser.

```
clasp open --webapp
? Open which deployment? (Use arrow keys)
❯                               @HEAD - AKf...h2S
```

If everything worked, you should see the <b>Hello Apps Script!</b> welcom page.