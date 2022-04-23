# blog.sh

`blog.sh` is a minimal blog engine written by [Karl](http://www.karl.berlin/blog.html )

## Writing a post 

* Use [Markdown](https://www.markdownguide.org/basic-syntax/) as a syntax guide. How you structure the post is up to you. 
* Then send the markdown file to adam. 

## Build Process (to be ran each time adding new posts)

* Put blog posts as markdown files into `posts`
* Run `./blog.sh` and posts will show up in `build/index-with-drafts.html`
* Commit posts in git to add timestamps and have them show up in `build/index.html`
* Copy the content of `build` to webserver

**N.B.** To do this you have to have `markdown` installed, via `apt-install markdown`, as well as the python library [md2gemini](https://pypi.org/project/md2gemini/), and therefore python. 


## Testing process 

If you feel the need to check first how it looks before uploading, then proceed with the build process above,  `cd` into the `build` directory and run `python3 -m http.server 8000`. **N.B.** You must have python (3.x.x) installed. 

