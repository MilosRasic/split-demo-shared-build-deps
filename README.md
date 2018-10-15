# Shared build dependencies

Build dependencies for Split Demo apps and main project. This repo simply encapsulates all the packages that we would otherwise copy-paste into devDependencies of every project that can be ran using webpack-dev-server.

Packages that should go here are ones used by the main repo to build, test or provide dev tools when the application is run in local environment using webpack-dev-server.

## Usage

To add build deps to a project simply

```
yarn add @split-demo/shared-build-deps --dev
```

or

```
npm --save-dev @split-demo/shared-build-deps
```

with npm v3. Higher versions of npm will not flatten the dependencies correctly.

This package should never be symlinked because that would break flattening of node_modules.
