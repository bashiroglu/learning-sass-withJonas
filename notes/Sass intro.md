# SASS and CSS

There are two syntaxs in sass, sass and scss. scss is with {} and look like css with advantages of sass but sass is working without {}.

##### SASS set-up

Sass is the system where we write code, the the code will be compiled to css. Browser only will be aware of css code. Sass only makes our file easier and development process faster, give ablility to resuse code etc. Because of these reasons we prefer sass. In order to compile sass code we use sass-compiler which is built in node-sass package.
The code below shows compile from where to where and watch (-w), just in case for any changes in our main scss file. This becomes very handy in development process of application.

```
"node-sass sass/main.scss css/style.css -w"
```

in order to have code architechture we use several folder for our file and import all to our main sass file. Folder named like below:

1. abstracts (for mixen and function which doesn't contain any css code)
2. base (necessary value for our project)
3. components (components like button, form etc)
4. layout (for layout)
5. pages (for our pages)

##### SASS

In sass we can nest code blocks to have more clean code. if we want to nest 2 code blocks like li inside of ul it will be like this

```
ul {
     // code block
    li {
        // code block
    }
}

// will be compiled
ul {
        // code block
}
ul li {
        // code block
    }
```

but if we want .nav and nav-item class we don't have to write our code like above, even in this case we can use nesting

```
.header {
  height: 95vh;
  &__logo-box {
    position: absolute;
  }
}
this will be compiled
.header {
  height: 95vh;
}
.header__logo-box {
    position: absolute;
}
```

#### SASS fetures

- extend feature
