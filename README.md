# Function31.github.io

Documentation on how to contribute posts to this blog will be ready shortly!

# function31.github.io

## Getting Started
* fork this repo & clone down the forked repo from your GH

Then from terminal

* check if you have ruby: `ruby --version`  
  if you don't:
    1. run `brew update`
    2. install ruby `brew install ruby` (??)

* install ruby `gem install jekyll`
* install jekyll-paginate `gem install jekyll-paginate`
* install bundler `gem install bundler`  (??)

## Writing up your post
* Posts are written in markdown syntax (link to md syntax)
* Navigate to `_posts` and touch a new file with the following naming convention: `YYYY-MM-DD-your-post-title.md` where `your-post-title` is a shorthand title for your post and `YYYY-MM-DD` where YYYY is 4 digit year, MM is the 2 digit month, DD is the 2 digit day.

* Within `_drafts` find a template that best fits your post needs (text only, picture with text, video with text) and copy the text of that template file into your newly created post file

* Then write away, Hemingway!

### Additional notes
Adding an image:
Adding a video:
Adding links:


## After you've finished writing

* save the file
* from Terminal, run the command `jekyll serve` inside the directory to preview the site on a local server.
Note: running `jekyll serve` generates the `_site` folder created. Don't modify anything inside this folder!
* preview it with: packages > Markdownpreview ... `CTRL + SHIFT + M`
* Open `localhost:4000` to see a preview of the site.

* If everything looks as you'd like it to look, stop server and start the GIT Workflow described  below.
* If it doesn't, go back to your md file to make the desired changes. After changes are made, run `jekyll serve` to build the `_serve` folder with changes incorporated.
* Preview the site by navigating to localhost:4000
* If all looks good, stop server and do the below workflow
* If not, repeat the above directions again.

## GIT Workflow
* git add <your post file>.md, **DO NOT `git add .`**
* gc "<post title - any comments>"
* gpom
* create a pull request to function31.github.io

* function31 administrators will merge your pull requests within a day or two
* follow up recommendations
...feel free to slack out a message on the g31_function31 channel to remind us to approve also or dm Ben or Ji directly
