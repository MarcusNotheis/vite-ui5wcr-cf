# UI5 Web Components for React - Vite + TypeScript on Cloud Foundry

This repository demonstrates how you can deploy an app using Vite and UI5 Web Components for React to Cloud Foundry.
This repo is based on our [vite template]().

For running the app on Cloud Foundry, I recommend using the `[@sap/approuter](https://www.npmjs.com/package/@sap/approuter)` package.
The `xs-app.json` file contains all the routing and it is started via the package.json `start` script.

The `manifest.yml` contains all the Cloud Foundry specific settings like the buildpack which is used and the route for the application.

To deploy this example, follow these steps:

```bash
# install dependencies
npm install

# login to your cf account and choose your org and space
cf login

# run the build (generate the dist folder)
npm run build 

# deploy 🚀
cf push
```


## Getting Started

First, install the `node_modules`:

```bash
npm install
```

Then, run the development server:

```bash
npm run dev
```

## Run Tests

Run all component tests headlessly in Chrome:

```bash
npm run test
```

Open component tests in Chrome:

```bash
npm run test:open
```

## Learn More

To learn more about Vite and UI5 Web Components for React, please visit the following resources:

- [Vite Documentation](https://vitejs.dev/)
- [UI5 Web Components Documentation](https://sap.github.io/ui5-webcomponents/)
- [UI5 Web Components for React Documentation](https://sap.github.io/ui5-webcomponents-react/)
