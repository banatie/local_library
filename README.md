# local_library

## Create Skeleton Expressjs Project

## Setup Commands
### Run Node Server
```
npm run devstart(npm run serverstart)
```

## Model Definitions

## Route Path Definitions
* catalog/ — The home/index page.
* catalog/<objects>/ — The list of all books, bookinstances, genres, or authors (e.g. /catalog/books/, /catalog/genres/, etc.)
* catalog/<object>/<id> — The detail page for a specific book, bookinstance, genre, or author with the given _id field value (e.g. /catalog/book/584493c1f4887f06c0e67d37).
* catalog/<object>/create — The form to create a new book, bookinstance, genre, or author (e.g. /catalog/book/create).
* catalog/<object>/<id>/update — The form to update a specific book, bookinstance, genre, or author with the given _id field value (e.g. /catalog/book/584493c1f4887f06c0e67d37/update).
* catalog/<object>/<id>/delete — The form to delete a specific book, bookinstance, genre, author with the given _id field value (e.g. /catalog/book/584493c1f4887f06c0e67d37/delete).

## Tech Stack
### Mongoose
A npm module that controls MongoDB instance.

### ExpressJS
A nodejs web framework.

### Pug
A Template engine.

## npm Modules
express-generator(npm install express-generator -g)
nodemon(npm install nodemon -g)
async(npm install async)
luxon(npm install luxon)
express-valdator(npm install express-validator)


## ExpressJS Setup
```
express <app name> --view=pug
cd <app name>
npm install
```
then, add the following code to script section in package.json
```
  "scripts": {
    "start": "node ./bin/www",
    "devstart": "nodemon ./bin/www",
    "serverstart": "DEBUG=express-locallibrary-tutorial:* npm run devstart"
  },
```
