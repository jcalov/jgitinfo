# README

The `jgitinfo` package provides a personally preferred configuration for the great package [gitinfo2](https://ctan.org/pkg/gitinfo2) written by Brent Longborough.

The files in the directory `git_hooks` of this repo are copies of the file `post-xxx-sample.txt` from the original [gitinfo2 repo](https://github.com/Hightor/gitinfo2) as you can also see in the source code of these files.

If you want the full configuration possibilities of the package [gitinfo2](https://ctan.org/pkg/gitinfo2), you have to use the original package.
Perhaps you will then run into a problem with an annoying bullet in the watermark text.
How you can build your own workaround for this problem is described there: [https://github.com/Hightor/gitinfo2/issues/20](https://github.com/Hightor/gitinfo2/issues/20).

## Package options

`silent`:
Show dirty flag in normal git info watermark (no prominent notice if repo is dirty). Dirty means: you have uncommited changes.

`verbose-not-installed`:
Show prominent info in watermark if git hooks are not installed. Don´t use this option if you use [git-latexdiff](https://gitlab.com/git-latexdiff/git-latexdiff).

## How to ensure watermark info if repo is dirty
The package only can know if the repo is dirty if one of the installed git hooks was invoked. So you have to ensure that you invoke one of them before compiling your latex document.

One possibility is to checkout a file that is in every branch of every repo and changes extremely rarely. Normally that file is `.gitignore`, so you can run `git checkout .gitignore` before every compile.

How you configure this in [TexStudio](https://www.texstudio.org) ist described in [section 1.3 of the TeXstudio user manual](http://texstudio.sourceforge.net/manual/current/usermanual_en.html#SECTION02a).

## Installation

* Copy the files from the repo folder `git_hooks` into your local repository folder `.git/hooks/`
* Make the files executable, e.g. with `chmod 755 .git/hooks/post-*`
* Ensure that you invoke one of the hooks before compiling your latex document (see previous section)

For more information see the [package documentation](http://mirrors.ctan.org/macros/latex/contrib/gitinfo2/gitinfo2.pdf) for the [gitinfo2](https://ctan.org/pkg/gitinfo2) package.
