Express Photo Application
=====================

----------------------------------------------------------------------------
##Step 00 - Preparation
----------------------------------------------------------------------------

##### Pre requirements
* [NodeJS](https://nodejs.org/)
* [Git](https://git-scm.com/downloads)
* [SourceTree](https://www.sourcetreeapp.com/)
* [MongoDB](https://www.mongodb.org/downloads)

##### Tools
* Editor: [Cloud 9](https://c9.io/)
* Sass compiler: [Koala](http://koala-app.com/)

###Preparation

##### Install global Node packages

    // install global packages
    npm install -g grunt-cli
    npm install -g express
    npm install -g express-generator
    npm install -g nodemon
    
#####Create the project skeleton
 
    // Add the -e flag to use the EJS template engine
    express -e photos
    cd photos

##### Install local Node packages

    npm install mongoose --save
    npm install mongodb --save
    npm install colors --save
    npm install ejs --save
    npm install

##### Adding git support

 1. Init the local repository `git init`
 2. Create new git repository on github
 2. Follow the instructions and add the git remote to this local repository
 3. Create the .gitignore file to ignore all the ___node_modules___

#####Installing MongoDB
 Donload mongoDB and copy the files in the bin folder within
 to wherever you want Mongo to live, and you're done. You've installed Mongo

----------------------------------------------------------------------------

* Test the application

    DEBUG=photos:* npm start

>
Open Browser in http://127.0.0.1:3000
You should now see the Welcome page

----------------------------------------------------------------------------
###Step 01 - Add data & routes
----------------------------------------------------------------------------

1. Add photos (data) to display
>   Create new file: **routes/photos.js** and fill in your data

2. Add photos (route)
>   Create new file: **routes/photos.js** and fill in your data

----------------------------------------------------------------------------
###Step 02 - Add photos (route + view)
----------------------------------------------------------------------------

1. Edit routes/photos.js and add a list function to list (display) the images
2. Create new file views/photos.ejs which will be served as our HTML page to display the images
3. Edit app.js and add the photos as required module
4. Edit app.js and set the photos list as our default view
5. restart the node server and reload the page

----------------------------------------------------------------------------
###Step 03 - Adding the upload form
----------------------------------------------------------------------------

##### Install **multer** for express v4.X

    npm install --save multer

- Create file models/Photo.js
- Creating a photo upload form (views/photos/upload.ejs)
- Add the new routes to app.js
- Add the upload form (views/photos/upload.ejs)
- Adding photo submit route definition
- Add photo upload destination settings (app.js)
- Showing a list of uploaded photos (Modified list route)
- Modified view to use settings for photos path
