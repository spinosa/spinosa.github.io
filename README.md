the_code_isthe_blog_
=================

What's going on here?  Welp, I'm trying to create a nice way to blog where the primary focus of the blogging is code.  Including code with tumblr kinda sucks.  But GitHub Pages has a strong focus on code....


Blogging about Code
=================

I'm limiting myself to two resources: git and GitHub Pages.  My high level goals are:
1.  A simple "container site" hosted at spinosa.github.io (to move to custom domian thecodeistheblog.com eventually)
2.  Each "post" on that site is actually it's own repository

Here's the current plan I'm working on to accomplish that:
1.  Set up the "container site"
  1.  Create a personal repo that GH will publish: spinosa.github.io
  2.  Use the GHPages site generator to get a basic up and running for spinosa.github.io
  3.  Set up a custom domain (later)
2.  Create my first "post repository"
  1.  Create a standard repo with some code, README.md and LICENSE
  2.  Manually create `gh-pages` branch in that repo with a single file: index.html
  3.  This file will become the blog post...
3.  Publish that post
  1.  Add the "post repository" as a submodule of the "container site"...
  2.  The submodule needs to track the `gh-pages` branch
  3.  The submodule needs to be added at the root of spinosa.github.io in a directory called `blog-post-name`

What did we just do?
-----------------
>  Publishing as outlined above will create "/blog-post-name/index.html" in the spinosa.github.io repository
>  Jekyll (the engine processing GHPages) will make that available as "http://spinosa.github.io/blog-post-name"


What's next?
-----------------
> Did it work?
> If so...
1.  update my documentation on *how* to accomplish this
2.  add some content to spinosa.github.io/index.html about what's going on here
3.  write the actual blog post about my code
4.  link to the blog post from spinosa.github.io/index.html
5.  write another blog post about this form of blogging =]