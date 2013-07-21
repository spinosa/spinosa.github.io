the_code_is_the_blog
=================

What's going on here?  Welp, I'm trying to create a nice way to blog where the primary focus of the blogging is code.  Including code with tumblr kinda sucks.  But GitHub Pages has a strong focus on code....


Blogging about Code
=================

I'm limiting myself to two resources: git and GitHub Pages.  My high level goals are:
1.  A simple "container site" hosted at [spinosa.github.io] (to move to custom domian [thecodeistheblog.com] eventually)
2.  Each "post" on that site is actually it's own repository

Here's the current plan I'm working on to accomplish that:

1. [x] Set up the "container site"
  - [x] Create a personal repo that GH will publish: [spinosa.github.io]
  - [x] Use the GHPages site generator to get a basic up and running for [spinosa.github.io]
  - [x] Set up a custom domain (later)
 
2. [x] Create my first "post repository"
  1. [x]  Create a standard repo with some code, README.md and LICENSE
  2. [x]  Manually create `gh-pages` branch in that repo with a single file: index.html
  3. [x]  This file will become the blog post...

3. [x]  Publish that post
  1.  There are two ways to publish...
    1.  It's already published!
      *  The `gh-pages` branch above with the `index.html` file is available at [http://<username>.github.io/normal-repo-name]
    2.  Customize the post name...
      1.  Add the "post repository" as a submodule of the "container site"...
        *  `git submodule add -b gh-pages https://github.com/<username>/<normal-repo-name> <blog-post-name>`
        *  You file will now _also_ be available at [http://<username>.github.io/<blog-post-name>]


We did it!
-----------------
What's Left?
-----------------
1.  Get a nice jekyll template working on the container site
2.  Get that template working for the post repository
3.  Probably more stuff, but I gotta bounce right now... getting yelled at...


What's next?
-----------------
* Did it work?
* If so...

1.  update my documentation on *how* to accomplish this
2.  add some content to spinosa.github.io/index.html about what's going on here
3.  write the actual blog post about my code
4.  link to the blog post from spinosa.github.io/index.html
5.  write another blog post about this form of blogging =]
