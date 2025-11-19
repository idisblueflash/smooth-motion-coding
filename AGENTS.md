# Initial Guide

## node.js
verify node.js is installed with `node -v`, install it if there's no node on the system.

## create new project
follow the docs/agent/configure-project.md to run the command to create a new project
select TypeScript for default language, and the FFmpeg as default exporter.

## install packages
after init, go inside the folder with `cd my-canvas` to install the dependencies with `npm install`

## start the editor
`$ bash -lc 'cd my-canvas && npm start >/tmp/motion_start.log 2>&1 & pid=$!; sleep 6; open http://localhost:9000/;'`
start the server in the background, wait briefly for it to be ready, then open the default browser pointing to localhost, and finally stop the server to avoid leaving processes running. Using a bash script that runs npm start in the background, waits a few seconds, opens the browser via open(Mac OS) http://localhost:9000/, and then provide user a command to kill the server.
