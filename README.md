# README

The `jgitinfo` package provides a personally preferred configuration for the great package [gitinfo2](https://ctan.org/pkg/gitinfo2) written by Brent Longborough.

If you want the full configuration possibilities of the package [gitinfo2](https://ctan.org/pkg/gitinfo2), you have to use the original package.
Perhaps you will then run into a problem with an annoying bullet in the watermark text.
How you can build your own workaround for this problem is described there: [https://github.com/Hightor/gitinfo2/issues/20](https://github.com/Hightor/gitinfo2/issues/20)

## Package options

`silent`:
Show dirty flag in normal git info watermark (no prominent notice if repo is dirty). Dirty means: you have uncommited changes.

`verbose-not-installed`:
Show prominent info in watermark if git hooks are not installed. Don´t use this option if you use [git-latexdiff](https://gitlab.com/git-latexdiff/git-latexdiff).
