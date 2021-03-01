---
layout: post
title:      "Note Taker App Frontend"
date:       2021-02-28 23:04:07 -0500
permalink:  note_taker_app_frontend
---


I began building the frontend of my application to ensure that my seed data is being passed in to the frontend.

I'm going to be using react.js to build my frontend functionality. I want to build a collapsible form that will allow a user to enter in the category for their note, the subject, and the note itself. 

I implemented create-react-app note-taker-app-frontend in the terminal and cd into my folder and began coding.

I began importing in react and react-dom and building my components. I also started building my store using provider when I ran into npm installer issues. Provider.js can't be found. Tried deleting the package-lock.json and node_modules and re-running npm install, but began receiving a different error. 

```
Module not found: Can't resolve 'react' in '/root/code/labs/Projects/javascript/practice/note_taker_app_main/note_taker_app_frontend/node_modules/react-redux/es/components'
^C
```

Troubleshooting these issue is fun because it gives me a chance to use my troubleshooting skills. I'm receiving the Maximum call stack size exceeded when running npm install. Currently, using stack over flow and google as a resource. Going to tear my code apart piece by piece until I find a solution.

![Imgur](https://i.imgur.com/czNiWGI.png)
