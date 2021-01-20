<div align="center" markdown="1">

<img src="https://celerik.com/wp-content/uploads/2019/12/celerik-1.svg" alt="Celerik" width="300">


# Ionic React + Capacitor template
<br>
<img src="ionic-react-capacitor.png" alt="Celerik" width="300">

</div>

## What's it

*@celerik/ionic-react-boilerplate* provides a code baseline for creating hybrid mobile applications based on Ionic React framework using Capacitor as it's default core, the set of tools included on this project defines a group of rules, linter conventions and a default tool for creating new components.
## What is included
- Sass and Scss support
- TypeScript support
- Storybook for components, docs [here](https://storybook.js.org/docs/react/get-started/introduction)
- WebStorm/PhpStorm support
- Eslint + Prettier Rules

## Requirements
- NodeJs >= 14.x
- A javascript package manager such as Npm or Yarn (Yarn preferred)

## Quick start
- Download this template [here](https://github.com/celerik/ionic-react-boilerplate/archive/master.zip)
- Extract it and rename the folder with your project's name
- Modify package.json to match your app name
```
cd "folder name"
yarn install 
ionic serve 
```
## Adding new components to the project
In order to standardize components creating generate-react-cli.json contains the information to create Components, Pages and Layouts and their associates
- Creating a component:
```
npx generate-react-cli component ComponentName 
```
- Creating a page or a layout:
```
npx generate-react-cli component PageName  --type=page
npx generate-react-cli component LayoutName  --type=layout
```
these commands will create the new component in a sub-folder located inside these folders depending on the type:
- ./src/components
- ./src/pages
- ./src/layouts

The root folder can also be manually specified by using --path parameter
```
npx generate-react-cli component PageName  --type=page --path=src/pages/some-inner-folder
npx generate-react-cli component LayoutName  --type=layout --path=src/layouts/some-inner-folder
```
The output will be inside "./src/pages/some-inner-folder/PageName/" for the first case
## Adding native platform project folders
To add iOS or Android folder you simply have to execute the command
- npx cap add "platform":
```
npx cap add ios
npx cap add android 
```

## API and examples

- Check out tutorials on Celerik's blog [here](http://celerik.com).

## License

*@celerik/ionic-react-boilerplate* is licensed under the [MIT license](LICENSE).

## How to contribute
TODO: Check out the contributing guide [here](CONTRIBUTING.md).
