# projectTemplate

File structure and tooling template for new projects

    Steps to setup tooling:

      1. Setting up your project:
         A. For local only projects:
              - Git clone this project to the desired directoy (cmd: git clone
              https://github.com/gorsuchtim/projectTemplate

              - Rename the folder to your project name

              - In the command line run npm install to install all dependencies
              into your project

          B. For git projects
              - In github, create a new repository
              - Git clone that repo to your system (git clone repoURL)
              - Copy the contents of this projectTemplate repo to that empty folder in your workspace/editor

        2. Using the tool:
          Use npm install to install all of the tool dependencies listed in package.json

          Here is a list of available scripts and what they'll do (you can see these in package.json):
            1. npm run dev: this will load up a local development server in the browser.
              a. Note: Parcel has a built-in sass bundler so all css is imported via App.js through shared.scss.

            2. npm run prettier: if you don't have the Prettier extension enabled/installed in your editor, this will format your code to our team standard code format.

            3. npm run lint: this will run eslint on your JS to check for errors or inconsistencies with how we want to structure our javascript.

            4. npm run format: this is a combo script: this will FIRST run lint to check for errors and IF THERE ARE NO ERRORS it will format your code using Prettier.

            5. npm run build: run this script when you're ready to create your minified/packaged javascript file to load into CTE/Production
              a. The build script will first run lint to ensure no errors/inconsistencies and then will format the code via Prettier before providing a minified/packaged file
              b. If errors/inconsistencies exist in the code the build will fail.  Once the errors are resolved, build will run as expected and provide your file.

          The repo includes a Utilities.js file available in /src/js/Components/Utilities
