# Electron React TypeScript Template

This project is a template for creating an Electron application based on Electron Forge using React and TypeScript. The project is pre-configured to kickstart development, providing a basic structure and configuration.

## Features

- **React**: Harness the power of React to build the user interface for your Electron application.
- **TypeScript**: All code is written in TypeScript to enhance readability, support, and static typing.
- **Webpack**: The project is built using Webpack, providing efficient code organization and optimization.
- **Electron**: The project is ready to use with Electron, allowing you to easily create cross-platform desktop applications.

## How to use

*Clone this repository locally:*

``` bash
git clone https://github.com/vladislavrupets/electron-react-typescript-template.git
```

*Install dependencies with npm:*
   
``` bash
cd electron-react-typescript-template
npm install
```

## App packaging

*Package the application (for any platform)*

``` bash
npm run package
```
## Notes

1. To bridge Electron's and React together, you need to use a special script called a preload in `./src/electron/preload.ts`.
2. You can add external resources (such as configuration files) to the project. Place the required file in the path `./src/extraResources/your-extra-file`. The path to external resources can be changed in `./src/forge.config.ts`:
```javascript
  const config: ForgeConfig = {
  packagerConfig: {
    asar: true,
    extraResource: ["./src/extraResources"],
    icon: "./public/icon",
  },
  ...
```
3. For additional questions, please refer to the [official Electron documentation](https://electronjs.org/docs) and [Electron Forge documentation](https://www.electronforge.io/docs).


