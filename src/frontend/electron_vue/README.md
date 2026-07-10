# Munt Electron Wallet

## Project setup
```
yarn
```

### Copy os specific unity lib to src/unity folder
```
yarn libunity:copy
```
By default this downloads from the GitHub release tag that matches `package.json` version (for example `v3.0.7`).
To force a different release tag, set `MUNT_RELEASE_TAG` before running the command.

### Compiles and hot-reloads for development
```
yarn electron:serve
```

### Compiles and minifies for production
```
yarn electron:build
```

### Lints and fixes files
```
yarn lint
```
