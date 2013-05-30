# JKL

A light-weight Jekyll v1.0 blog scaffolding that's ready to deploy after setting up one 
config. Still under development. Pull requests encouraged && accepted. 

# Get Started
```
git clone git@github.com:mrmrs/jkl.git && cd jkl && rake dev
```

That should do the trick. More verbose explanations below.



## Rake tasks

#### rake dev
```
jekyll serve --watch
```

This sets up a jekyll server for dev on port 4000. Site is regenerated everytime you save a file. 
NOTE: Changing _config.yml will require a restart of the jekyll server to see changes.
To restart server, go to terminal tab that server is running in then press
```
ctrl+C ⇧  enter
```

#### rake sass
```
sass --watch _sass:css 
```

Starts Sass polling to regenerate css on file save. 

#### rake minify
```
sass --watch _sass:css --style compressed
```

Starts Sass polling to regenerate css on file save - minifies the output.

## Notes
Example posts are in jkl/_posts/
There are two layouts, one for posts, one for other pages. Layouts are stored, creatively, 
in jkl/_layouts/ Folders that begin with an underscore are not copied over to
_site.

