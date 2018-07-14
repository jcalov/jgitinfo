# README

The `jgitinfo` package provides a personally preferred configuration for the great package `gitinfo2` written by Brent Longborough: [https://ctan.org/pkg/gitinfo2](https://ctan.org/pkg/gitinfo2)

If you want the full configuration possibilities of the package `gitinfo2`, you have to use the original package.
Perhaps you will then run into a problem with an annoying bullet in the watermark text.
How you can build your own workaround for this problem is described there: [https://github.com/Hightor/gitinfo2/issues/20](https://github.com/Hightor/gitinfo2/issues/20)

## Package options

`silent`: use this flag in following cases:

* No prominent notice if repo is _dirty_ (you have uncommited changes)
* You don´t want have a watermark if you don´t use git or have installed git hooks as described in the manual for the package `gitinfo2`. In this case, you maybe don´t want to use this package ;-)
