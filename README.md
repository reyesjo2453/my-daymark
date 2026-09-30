# Daymark

Daymark is a personal task manager inspired by the workflow John wants from Todoist, with its own interface and implementation. This first build is a responsive progressive web app that can be hosted as a static site.

## In this build

- Inbox, Today, Upcoming, Completed, and Personal, Work, and Home project views.
- Task creation and editing with due dates and four priority levels.
- Search, sorting, completion, and deletion.
- Local browser storage with JSON import and export for backups or later migration.
- Typed assistant commands and browser speech-to-text for task capture.
- Offline app shell and installable PWA metadata.

## Current limits

- Tasks are stored in the browser on this device. They do not yet sync across devices.
- The assistant is a local command demo, not a connected AI model.
- Automatic one-way sync to ChatGPT is not yet connected. GitHub Pages can host the app files, but a separate authenticated backend/MCP data path is required for ChatGPT to read saved tasks. No task data or credentials should be published into the source repository.
- This build does not yet implement notifications, calendar view, recurring schedules, or shared projects.

## Run locally

Serve this folder from a local web server (the service worker and microphone require a secure context such as `localhost` or HTTPS). Open the served page in a modern browser. Browser speech recognition availability depends on the browser and microphone permission.

## Data backup

Choose **Export** to download a JSON backup. Choose **Import** to restore a Daymark JSON backup. Import replaces the tasks currently saved in that browser.

## Hosting

The static files can be deployed with GitHub Pages. Keep task records and authentication credentials out of the public repository. ChatGPT sync requires a separately deployed, authenticated service and connected read tools.
