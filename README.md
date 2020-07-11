# Sharity Front End

Web application that provides a clean way to manage de donation administration of a charity event.

## Technologies

The technologies used to develop the project are the following:

* Node.js
* Svelte
* Bootstrap 4
* Routify

## Project Setup

To start working on the project is needed to have installed node.js in the computer environment

### Node.js

To get started with the node.js installation, is just needed to go to the node.js website and follow the instructions that it provides.

### Package.json

After installing node, is necessary to install the node dependencies used in this project, just run **npm install** node after cloning the repository locally on the computer.

## Technology Management

### Svelte

Svelte is used as a framework/compiler to create components and manage code for the website. Svelte is also used to make the website dynamic so it receives data from the REST API.

### Routify

Routify is an svelte librarie made to handle routing with svelte.

## Recommendations

The following recommendations aren't needed to work on the project.

Install svelte3 snippets to facilitate the development enviroment in Visual Studio Code.

## Configurations

Svelte-Carousel needs a minimum amount of slides to show per page, the defaul configuration is 3 slides per page, if not configurated correctly it will print out an error. An example of this application would be the following: 

```html
<Carousel perPage="Number of slides per page">
<Carousel/>
```

## FAQ

Installing svelte inside windows sometimes could be problematic, if that's the case is easier installing Linux Subsystem and setting up there the svelte project.

To build the project for deployment just **run npm run** build in the terminal so the live-reload turns off
