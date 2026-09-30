# Daymark

Daymark is a personal task manager with an Inbox, Today, Upcoming, Completed, and project views. It supports task priorities, due dates, search, sorting, voice capture through browser speech recognition, and JSON backup import/export.

## Two versions

- **GitHub Pages preview:** [Open Daymark](https://reyesjo2453.github.io/my-daymark/). This public static edition saves tasks in the current browser only.
- **Private synced edition:** [Open connected Daymark](https://fitness-connect.reyesjo2453.chatgpt.site/daymark). Sign in with ChatGPT. Tasks sync to the private Fitness Connect account and can be read in ChatGPT while its personal plugin is connected. Sync runs after edits, when reopened, and while the page is visible.

The app source is public, but task records and sign-in data are not stored in this repository. The private edition uses Fitness Connect's authenticated backend. The assistant embedded in the app currently handles a few local task commands; ChatGPT can use the connected read tools to review synced tasks.

## Features

- Inbox, Today, Upcoming, and Completed task views.
- Personal, Work, and Home projects.
- Add, edit, complete, and delete tasks with due dates and four priority levels.
- Search and sort tasks.
- Typed task commands and browser speech-to-text capture.
- JSON import and export for backups.
- Installable progressive web app shell for the public preview.

## Run locally

Serve this folder from a local web server. A secure context such as `localhost` or HTTPS is needed for the service worker and microphone. Browser speech recognition availability depends on browser support and microphone permission.

## Current limits

The public GitHub Pages version is browser-only and does not sync with ChatGPT. Use the private connected edition above for automatic sync and ChatGPT task reading. Recurring schedules, notifications, calendar views, shared projects, and full AI chat inside the app are not implemented yet.
