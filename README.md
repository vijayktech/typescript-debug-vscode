1. Create a folder
2. initialise the project below commands

```
## create package.json
npm init -y  

# Install typescript
npm install --save-dev typescript

## Create a tsconfig.json
tsc --init
Note : check the content inside tsconfig.json

# Add script options in package.json
"scripts": {   
    "build" : "tsc",
    "prestart": "npm run build",
    "start": "node out/app.js"
  }

# Add the vscode below snippet to VSCode
      {     
            "program": "${workspaceFolder}\\src\\app.ts",
            "preLaunchTask": "npm: build",
            "sourceMaps": true,
            "smartStep": true,
            "internalConsoleOptions": "openOnSessionStart",
            "outFiles": [
                "${workspaceFolder}/out/**/*.js"
            ]
        }


```
