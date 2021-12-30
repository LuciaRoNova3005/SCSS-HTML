# HTML || SASS || RESPONSIVE

This project consists of the creation of a page and its adaptation for the different tablet and mobile devices.

![image](https://user-images.githubusercontent.com/81588630/124919114-1d369f80-dff6-11eb-83aa-90c5ee2d04c6.png)


This project includes an HTML template engine, the SASS preprocessor and a local server and many other things, this helps us to work more comfortably, it automates tasks.

There are 3 types of files and folders:

-The files that are loose in the repository root, like gulpfile.js, package.json... are the project configuration.

- The `src/` folder: these are the web page files, such as HTML, CSS, JS...
- The `public/` and `docs/` folders,which are automatically generated when we start the project. The Kit reads the files inside `src/`, processes them and generates them inside `public/` and `docs/`.

## Quick Start Guide

> ** NOTE: ** Install previously [Node JS](https://nodejs.org/) to work with this repo:

### Steps to follow to start the project from your computer::

1. Create a new repository and add the downloaded files.
1. ** Open a terminal ** in the root folder of your repository.
1. ** Install the local dependencies ** by executing the command in the terminal:

```bash
npm install
```

Once we have installed the dependencies, we are going to start the project. ** The project must be started every time you open it ** To do this, execute the command:

```bash
npm start
```

Este comando:

- **Open a Chrome window and show the web page**
- Also ** observe ** all the files that are inside the `src /` folder, so that every time you modify a file ** it refreshes your page in Chrome **.
- It also ** processes the ** HTML, SASS / CSS and JS files and ** generates and saves them in the `public /` ** folder. For example:

After executing `npm start` you can start to edit all the files that are inside the`src /`folder and program comfortably.

### Steps to publish the project on GitHub Pages::

To generate the page for production run the command:

```bash
npm run docs
```

And then:

1. Upload the `docs /` folder that was just generated to your repo..

```bash
git add -A
git commit -m "commit message"
git push
```

Also, the commands:

```bash
npm run push-docs
```

o

```bash
npm run deploy
```

They are a shortcut that generates the production version and pushes the `docs /` folder at once.

## File flow with Gulp

These Gulp tasks produce the following file stream:

![Gulp flow](./gulp-flow.png)

## `gulpfile.js` y `config.json`

Our ** gulpfile.js ** uses the configuration file `config.json` with the paths of the files to generate / observe.

In this way we separate the actions that are in `gulpfile.js` from the configuration of the actions that are in` config.json`.

## Folder structure

```
src
 ├─ images
 ├─ js // the files in this folder are concatenated in the main.js file and this is saved in public/main.js
 |  ├─ main.js
 |  └─ events.js
 ├─ scss
 |  ├─ core
 |  ├─ layout
 └─ html
    └─ partials
```

## Something is missing??

Any questions or suggestions or advice will be well received!
