# link to the deployed application

https://example-frontend-lzvy.onrender.com

# example-frontend

This project is created to help learn docker configurations for frontend projects. The README starting from "Prerequisites" is written without Docker in mind. I have modified this according to the instructions and created the Dockerfile

# Prerequisites

Install [node](https://nodejs.org/en/download/). 

Example node install instructions for LTS node 16.x:
```
curl -sL https://deb.nodesource.com/setup_16.x | bash
sudo apt install -y nodejs
```

Check your install with `node -v && npm -v`

Install all packages with `npm install`

# Starting in production mode

First, you need to build the static files with `npm run build`

This will generate them into `build` folder.

An example for serving static files:

Use npm package called serve to serve the project in port 5001:
- install: `npm install -g serve`
- serve: `serve -s -l 5001 build`

Test that the project is running by going to <http://localhost:5001>
