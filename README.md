# My Sass Workflow

![Mike](http://www.mikejakobsen.com/mike.png)

My Sass workflow

```
git clone https://github.com/mikejakobsen/Boilerplate.git /Sass-dir
```


[Github.com/mikejakobsen](http://www.github.com/mikejakobsen)
[Dribbble.com/mikejakobsen](http://www.dribbble.com/mikejakobsen)
[Twitter.com/mikejakobsen](http://www.twitter.com/mikejakobsen)


## Main syntax

```SCSS
.block {
    /* CSS declarations for `.block` */

    &__element {
        /* CSS declarations for `.block__element` */
    }

    &--modifier {
        /* CSS declarations for `.block--modifier` */

        &__element {
            /* CSS declarations for `.block--modifier__element` */
        }
    }
}
```

As much as possible, i try to stick with the [7-1 architecture pattern](http://sass-guidelin.es/#architecture) and sticking to [Sass Guidelines](http://sass-guidelin.es) writing conventions, and use the [BEM Syntax](http://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/)


## Using the indented syntax

This boilerplate does not provide a `.sass` version as it would be painful to maintain both versions without an appropriate build process. However, it is very easy to convert this boilerplate to Sass indented syntax.

Clone it, head into the project and then run:

```
sass-convert -F scss -T sass -i -R ./  && find . -iname “*.scss” -exec bash -c 'mv "$0" “${0%\.scss}.sass"' {} \;
```
