---
layout: inner   # do not change this value
comments: true  # do not change this value

title: "An Express Application"  # Rename this with the title of your post & surround with double quotes
date: 2016-09-07 12:37 # Date and military time
author: Sam Persian # Your name here ie Ji Kim
tags: js node express # tags are separated by whitespace, so use single words.
lead_text: "Create an express application." # Surround with double quotes. Tag lines will appear above the content of the post within each post.
---

# Today I'm going to show you how to make a basic express application.

### For this to work, both node and npm must be installed on your machine.

#### Now, lets begin.

1. Open your terminal. Now create a new project folder and cd into it.
  ```
  / > mkdir folder-name && cd folder-name
  ```
1. Create a package.json file with the defalt settings using npm.
  ```
  /folder-name > npm init
  ```
1. Install express along with all other node modules.
  ```
  /folder-name > npm install express -S
  ```
1. Create an index.js file in your project folder. Notice that this corresponds to the "main" value in your package.json file.
  ```
  /folder-name > touch index.js
  ```
1. Open your app.js file in a text editor. On the first line of the file, you're going to need to bring in the express module.
  ```
  const express = require('express');
  ```
1. Create the app itself.
  ```
  const app = express();
  ```
1. Next, specify the port you would like your app to run on.
  ```
  const port = 3000;
  ```
1. Now, you are going to set up your app to handle a basic GET request to your app.
  ```
  app.get("/", function(request, response, next) {
    response.send("This is an app running on an express server.");
  });
  ```
1. Tell your app to listen on the port you specified.
  ```
  app.listen(port);
  ```
1. Finally, go back to your terminal and start up your app!
  ```
  /folder-name > nodemon
  ```
1. Test that your app is running. Open a browser and go to (make a GET request to) http://localhost:3000. In your browser window you should see the response: ```This is an app running on an express server.```

### Congrats you have now setup a basic express application.

## Here are ALL of the commands in order.

#### In your terminal:

```
/ > mkdir folder-name && cd folder-name
/folder-name > npm init
/folder-name > npm install express -S
/folder-name > touch index.js
```

#### In your index.js:

```
const express = require('express');
const app = express();
const port = 3000;
app.get("/", function(request, response, next) {
  response.send("This is an app running on an express server."); });
app.listen(port);
```

#### Back in your terminal:

```
/folder-name > nodemon
```

#### Go to http://localhost:3000 in a web browser to see your app running!
