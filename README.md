# Blazor Dashboard App

This sample application showcases how easy it is to plug the Telerik Blazor components in your layout, data and models. It is insipred by other similar dashboard apps for [Vue.js](https://github.com/telerik/vue-dashboard) and [Angular](https://github.com/telerik/ng2-dashboard).

## What's Inside

* `Bootstrap` for the layouts
* the [Telerik Blazor components](https://www.telerik.com/blazor-ui) for the UI elements
* customized SASS variables for Bootstrap
* the Telerik Bootstrap SASS theme to also utilize those variables
* `Gulp` to fetch the SASS dependencies, build them and minify the output
* dummy data, because, at the time of writing, the [Octokit.NET](https://github.com/octokit/octokit.net) package does not work under Blazor due to [issues with async requests](https://github.com/aspnet/AspNetCore/issues/9125)

## How to Run Locally

To run this app locally, you need:

* .NET Core 3 Preview 6
* Visual Studio 2019 Preview
* Node.js

### One-time Installation

While the compiled CSS is commited in the repo and the app can run as-is, if you want to run the tasks yourself, you need to perform the procedure below. Alternatively, remove `gulpfile.js` and `package.json` from the project.

To build the dependencies, ensure you can build the SASS modules by:

1. open `PowerShell` as `Administrator`
1. execute `npm install --global --production windows-build-tools`
1. execute `npm install -g node-gyp`
1. from the command inside the project folder (where the `packages.json` file is), execute `npm install`

### Usual Run

1. open the `sln` file with VS 2019 Preview
1. press `F5`
