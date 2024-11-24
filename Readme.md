# Node.js Aur Backend Series

This is a video series on creating a backend with JavaScript.

## Step 1: Initialize a Node.js Backend
To create a new Node.js project, run:
```bash
npm init
```

## Step 2: Create a `src` Folder
Organize your project by creating a `src` folder:
```bash
mkdir src
```

## Step 3: Create Essential Files Inside `src`
Inside the `src` folder, create the following files:
```bash
touch src/app.js src/constants.js src/index.js
```

### Note:
To use the `import` keyword for module imports, add the following to your `package.json`:
```json
"type": "module"
```

## Step 4: Enable Auto-Restart for the Server
Install `nodemon` for auto-restarting the server after saving changes:
```bash
npm install -D nodemon
```
Add a script to your `package.json`:
```json
"dev": "nodemon src/index.js"
```

## Step 5: Create Project Structure
Create the following folders for better project organization:
```bash
mkdir controllers db middlewares models routes utils
```

## Step 6 (Optional): Install Prettier
To ensure consistent code formatting, install Prettier as a dev dependency:
```bash
npm install -D prettier
```

## Step 7: Install Required Packages
Install essential backend packages:
```bash
npm install express mongoose dotenv
```

## Step 8: Database Connection
1. Write the database connection logic in `src/db/index.js`.
2. Import the database connection in `src/index.js`.

### Additional Note:
Since we are using `dotenv`, modify the `dev` script in `package.json` as follows:
```json
"dev": "nodemon -r dotenv/config src/index.js"
```

