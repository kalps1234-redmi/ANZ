# ANZ
ANZ_Demos

https://elm-dev.nxp.com/jazzop/form/login

// NX js
npx create-nx-workspace <your-project-name>

\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\

Custom Utilities

Original Office React monorepo project
======================================
npx create-nx-workspace nxpLauncherApp

1. what config setup/selected?

PS C:\Users\nxg04126> cd C:\Users\nxg04126\Downloads\Projects-NXP\              
PS C:\Users\nxg04126\Downloads\Projects-NXP> npx create-nx-workspace nxpLauncherApp
Need to install the following packages:
create-nx-workspace@17.1.3
Ok to proceed? (y) y

 >  NX   Let's create a new workspace [https://nx.dev/getting-started/intro]

√ Which stack do you want to use? · react
√ What framework would you like to use? · none
√ Integrated monorepo, or standalone project? · integrated
√ Application name · nxpLauncherApp
√ Which bundler would you like to use? · webpack
√ Test runner to use for end to end (E2E) tests · none
√ Default stylesheet format · scss
'git' is not recognized as an internal or external command,
operable program or batch file.
√ Enable distributed caching to make your CI faster · Yes

 >  NX   Creating your v17.1.3 workspace.

   To make sure the command works reliably in all environments, and that the preset is applied correctly,
   Nx will run "npm install" several times. Please wait.


failed multiple time. error was =""

then did this

PS C:\Users\nxg04126\Downloads\Projects-NXP> npm config set registry http://registry.npmjs.org/
PS C:\Users\nxg04126\Downloads\Projects-NXP> npm config set strict-ssl false  

PS C:\Users\nxg04126\Downloads\Projects-NXP> $env:NODE_TLS_REJECT_UNAUTHORIZED="0"
PS C:\Users\nxg04126\Downloads\Projects-NXP> npm config set registry http://registry.npmjs.org/
PS C:\Users\nxg04126\Downloads\Projects-NXP> npx create-nx-workspace nxpLauncherApp
(node:5308) Warning: Setting the NODE_TLS_REJECT_UNAUTHORIZED environment variable to '0' makes TLS connections and HTTPS requests insecure by disabling certificate verification.
(Use `node --trace-warnings ...` to show where the warning was created)

 >  NX   Let's create a new workspace [https://nx.dev/getting-started/intro]

√ Which stack do you want to use? · react
√ What framework would you like to use? · none
√ Integrated monorepo, or standalone project? · integrated
√ Application name · nxpLauncherApp
√ Which bundler would you like to use? · webpack
√ Test runner to use for end to end (E2E) tests · none
√ Default stylesheet format · scss
'git' is not recognized as an internal or external command,
operable program or batch file.
√ Enable distributed caching to make your CI faster · Yes

 >  NX   Creating your v17.1.3 workspace.

   To make sure the command works reliably in all environments, and that the preset is applied correctly,
   Nx will run "npm install" several times. Please wait.

✔ Installing dependencies with npm
✔ Successfully created the workspace: nxp-launcher-app.
✔ NxCloud has been set up successfully
'git' is not recognized as an internal or external command,
operable program or batch file.

 ——————————————————————————————————————————————————————————————————————————————————————————————————————————————————————— 


 >  NX   Nx CLI is not installed globally.

   This means that you might have to use "yarn nx" or "npx nx" to execute commands in the workspace.
   Run "yarn global add nx" or "npm install -g nx" to be able to execute command directly.


 >  NX   Distributed caching via Nx Cloud has been enabled

   In addition to the caching, Nx Cloud provides config-free distributed execution,
   UI for viewing complex runs and GitHub integration. Learn more at https://nx.app

   Your workspace is currently unclaimed. Run details from unclaimed workspaces can be viewed on cloud.nx.app by anyone  
   with the link. Claim your workspace at the following link to restrict access.

   https://cloud.nx.app/orgs/workspace-setup?accessToken=MDM3N2M1ZGEtZWNmMi00ZmZjLWE3MGItYjUzZmY0Zjc0NDAyfHJlYWQtd3JpdGU=


 ——————————————————————————————————————————————————————————————————————————————————————————————————————————————————————— 


 >  NX   First time using Nx? Check out this interactive Nx tutorial.

   https://nx.dev/react-tutorial/1-code-generation

PS C:\Users\nxg04126\Downloads\Projects-NXP> 

port Changes
added it in project.json file
serve section

        "port": 5050
		
		"serve": {
		  "executor": "@nx/webpack:dev-server",
		  "defaultConfiguration": "development",
		  "options": {
			"buildTarget": "nxp-launcher-app:build",
			"port": 5050
		  },
		}


steps to run/execute the project

1. build process === npx nx build nxp-launcher-app:build:development
2. run/serve process === npx nx serve nxp-launcher-app:serve:development


in project.json file
"baseHref": ".",


        "port": 4202 in serve section
		
		
		
		git config --global user.email "kalpana.bilagi@nxp.com"
  git config --global user.name "KalpanaB"
  
  PRMI-80 - 202312041330 - ELM Custom Utilities Launcher widget added
  
  npx nx run-many --target=serve --projects=login,user-management --parallel --maxParallel=100
  
  
  
  
  https://nx.dev/recipes/react/module-federation-with-ssr#setup-module-federation-with-ssr-for-angular-and-react
  


npx create-nx-workspace@latest


 >  NX   Let's create a new workspace [https://nx.dev/getting-started/intro]

✔ Where would you like to create your workspace? · myorg
✔ Which stack do you want to use? · none
✔ Package-based or integrated? · integrated
✔ Enable distributed caching to make your CI faster · Yes

  npx nx g @nx/react:host login --remotes=user-management,attriute-mapping
  
  
==================================================== final project setup ===================================================================
final project setup
reference - https://nx.dev/recipes/react/module-federation-with-ssr#setup-module-federation-with-ssr-for-angular-and-react

in your project folder cli

PS C:\Users\nxg04126\Downloads\Projects-NXP> npm config set strict-ssl false  
PS C:\Users\nxg04126\Downloads\Projects-NXP> $env:NODE_TLS_REJECT_UNAUTHORIZED="0"
PS C:\Users\nxg04126\Downloads\Projects-NXP> npm config set registry http://registry.npmjs.org/


npx create-nx-workspace@latest


 >  NX   Let's create a new workspace [https://nx.dev/getting-started/intro]

✔ Where would you like to create your workspace? · custom-utilities
✔ Which stack do you want to use? · none
✔ Package-based or integrated? · integrated
✔ Enable distributed caching to make your CI faster · Yes

select style as "scss"

after all setup done -> 
npm i (may be)

create a folder "apps"
cd apps
npx nx g @nx/react:host login --e2eTestRunner=none --remotes=user-management,attriute-mapping      (dont use --ssr)

before hosting host app ===
use npm i

npx nx build login:build:development
npx nx serve login:serve:development

==============================================================================================================================================

npx nx serve login --devRemotes=sharelibraries,usermanagement

npx nx build login --devRemotes=sharelibraries,usermanagement


nxf70775
i3h##UC#uyWK

PRMI-87-base-application-setup



i3h##UC#uyWK


proxy

  {
    "context": ["/UMService"],
    "target": "http://localhost:8100",
    "changeOrigin": true,
    "secure": false
  },
  
  
  
  {
    "context": ["/projects"],
    "target": "http://localhost:8100/",
    "changeOrigin": true,
    "secure": false
  }
  
  
  "userName":"nxf70775",
   "password":"/4Y+lIvKZF7bmAJnVq3ukQ==",
