# Developing an application with the MERN stack

Building a full stack application in JavaScript means that your development stack will be using mostly the same JavaScript APIs - but there are some differences.

---

## Requirements

We will be using:

1. GIT - for code management and collaboration

> Initialise with `git init`

2. NPM - for package management (dependencies)

> Initialise with `npm init -y`

## .gitignore

Don't forget to create a `.gitignore` file.

You don't want to include all files in your github repo.

For example, the `node_modules` folder can grow quite large (even into the GigaBytes). You do not need to upload this since your `package.json` file references all your node dependencies.

`.env` usually contains sensitive information (database passwords, secret keys) and should not be added to `git`.

You can build a `.gitignore` with [gitignore.io](https://www.toptal.com/developers/gitignore)

Or you can use the `.gitignore` file included [in this repo](./.gitignore)

## Frontend

React (or React Native)

[Dependencies](./frontend/dependencies.md)

[Structure](./frontend/structure.md)

## Backend

MongoDB (Mongoose), Express.js, Node

[Dependencies](./backend/dependencies.md)

[Structure](./backend/structure.md)