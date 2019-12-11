# AppsScript-HTML-Starter
<h2>Overview</h2>

Create and Host a website with Apps Script. Use HTML, CSS, and JavaScript to design your pages. Use `clasp` to push your code to Google Drive and to deploy your site to Google Cloud Platform.

This project uses npm to install clasp. The clasp CLI lets you work on Apps Scripts locally and then push and deploy changes from your Terminal or IDE.

<h2>Instructions</h2>

<h3>Clone the project and install clasp</h3>

```
git clone git@github.com:ChaddPortwine/AppsScript-HTML-Starter
cd AppsScript-HTML-Starter
npm install
```

<h3>Create a new Apps Script Web App</h3>

Use `clasp` to create a new blank Apps Script project. Set the type, title, and directory.
```
clasp create --type webapp --title "AppsScript-HTML-Starter" --rootDir ./AppsScript-HTML-Starter
```

<h3>Update .clasp.json with the Project ID</h3>

Run `clasp list` to find your new Apps Script project and its ID.

```
clasp list
AppsScript-HTML…     – https://script.google.com/d/1RP...zGV/edit
```

See the shortened ID highlighed in <font color=red>red</font> below. Copy the ID and use it to update .clasp.json.

https://script.google.com<font>/d/</font><font color=red>1RP...zGV</font>/edit

```
//.clasp.json

{"scriptId":"1RP...zGV"} // Add the ID here
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
- AKfycbwqkMbn8WgzrNrYl2x7-7c-MB5Xb9pRQJYmLt0GQCRemBnNAh5LKSLl9xytuXIieQKLEQ @1.
```
<h3>Open the Web Page</h3>

Run `clasp open` to open you web page in a browser

```
clasp open
? Open which deployment? (Use arrow keys)
❯                               @HEAD - AKfycbym-zNorir1fcgPP5kmFJD849MfWx6riJpwoFUskh2S
```