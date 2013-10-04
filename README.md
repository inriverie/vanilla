# Vanilla

Barebones starter files and directory structure for new web projects.

## Build

    mkdir [PROJECT] && cd [PROJECT]
    git init
    git add remote inriverie https://github.com/inriverie/[PROJECT].git
    git add remote vanilla https://github.com/inriverie/vanilla.git
    git pull vanilla master
    git add .
    git commit -m "Vanilla init."
    git push inriverie HEAD

## Stylesheets

`config.styl` controls the project style settings. Each page specific stylesheet (`[PAGE].styl`) should have a section dedicated to over-writing these settings on a page-by-page basis (shown below).

`[PAGE].styl` files can be started by copying the following template or pulling in from [this Gist](https://gist.github.com/inriverie/5021968).

    /*------------------------------------*\
        SETTINGS
    \*------------------------------------*/
    @import '../config'





    /*------------------------------------*\
        REDEFINE VARIABLES
    \*------------------------------------*/





    /*------------------------------------*\
        OBJECTS
    \*------------------------------------*/
    @import '../imports'





    /*------------------------------------*\
        PAGE SPECIFIC STYLES
    \*------------------------------------*/

## Dependencies

* [Codekit](http://incident57.com/codekit/) for all the heavy lifting,
* My CSS utility, [Morula](https://github.com/inriverie/morula),
* CSS is preprocessed with [Stylus](http://learnboost.github.io/stylus/),
* [Jade](http://jade-lang.com/) templating.