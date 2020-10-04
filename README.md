
# README.md Generator: Node.js and ES6+

## Description 
    
This is a command-line application that runs with Node.js that dynamically generates a README.md file based on input about your project. Check out the [`ExampleREADME.md`](https://github.com/esmailmb/Good-Readme-Generator/blob/master/README.md) in this repo as an example. 


## Table of Contents
* [Installation](#installation)
* [Usage](#usage)
* [Methodology](#methodology)
* [License](#license)
  

## Installation


To generate your own README, first run `npm install` in order to install the following npm package dependencies as specified in the `package.json`:
  * [`inquirer`](https://www.npmjs.com/package/inquirer) that will prompt you for your inputs from the command line 
  * [`axios`](https://www.npmjs.com/package/axios) to fetch your info from the GitHub API

The application itself can be invoked with `node index.js`.


## Usage 


![Gif demo of README-generator](readme-demo.gif)

When you run `node index.js`, the application uses the `inquirer` package to prompt you in the command line with a series of questions about your GitHub and about your project.

The application then takes your responses and uses `axios` to fetch your GitHub profile from the [GitHub API](https://developer.github.com/v3/), including your GitHub profile picture (avatar) and email.


Finally, `fs.writeFile` is used to generate your project's README.md file. Check out the [`ExampleREADME.md`](https://github.com/esmailmb/Good-Readme-Generator/blob/master/README.md) in this repo as an example. The lorem ipsum is generated thanks to [Social Good Ipsum](http://socialgoodipsum.com/#/).


## Methodology

The application utilizes modularization by separating the GitHub API call and generation of the markdown into separate modules: `api.js` and `generateMarkdown.js`, respectively, inside the `utils` folder.

The application also utilizes, as much as possible, syntax and paradigms introduced in ES6 and beyond, including `arrow functions`, `const`, `let`, template literals, and `async/await` to handle the `inquirer`, `axios`, and `fs.writeFile` promises.


## License

MIT License





 



