Amongst various other frontends, Munt has an electron based frontend that sits on top of our unified backend.
This makes contributing toward the user interface more accessible to a wider audience of developers.

To get started tinkering with the electron frontend and/or contributing changes, these are the required steps:
1. Install prerequisites yarn/npm/node/git
2. Check out a copy of the repository using `git`
3. Select an appropriate branch. For development purposes you should use the latest development branch
4. Change into `src/frontend/electron_vue` folder
5. Type `yarn` to install the depedencies
6. Type `yarn libunity:copy` to fetch the latest unified backend plugin
7. Type `yarn electron:serve` to launch the program

Notes:
* Development version runs in a different data directory (munt_dev) than your regular wallet
* You can't/shouldn't run both versions simultaneously unless you change the ports of one of them 

Troubleshooting:
* If you previously configured npm/yarn to use the Font Awesome Pro registry, remove that override so packages resolve from the default npm registry.
```
npm config delete "@fortawesome:registry"
npm config delete "//npm.fontawesome.com/:_authToken"
```
The electron and lite frontends now use Font Awesome Free packages, so no Pro license token is required for local development.
