# Create new Angular app 
* ng new app 
* cd app
* ng serve --open
### note:
* The ng serve command:
    * Builds the application
    * Starts the development server
    * Watches the source files
    * Rebuilds the application as you make changes 
* The --open flag opens a browser to http://localhost:4200.

# deploy Angular Apps to GitHub Pages
* Create your Github Repository
* Create a gh-pages branch on your local machine 
    * git branch gh-pages
    * git checkout gh-pages
* Install Angular CLI gh-pages:
    * npm i angular-cli-ghpages --save-dev
* Run Build 
    * ng build --prod --base-href "https://AwaabElamin.github.io/WebAppAwaab/"
* Deploy to gh-pages
    * npx angular-cli-ghpages --dir=dist/Project-name
    * You can find this in the angular.json file under defaultProject which is at the bottom of the file. If the project name is wrong, your App will not work; so if you are seeing any errors, check the angular.json to confirm if you used the correct project name
* Visit the App Page
    * https://AwaabElamin.github.io/WebAppAwaab/