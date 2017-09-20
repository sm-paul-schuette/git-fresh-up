# git fresh-up
This repository is meant to hold links and information to the short git fresh-up presentation.

## presentation
The [presentation] shows three catch-phrases in the work with git

- commit often
- perfect later
- publish once

## focus of this repo
This repo's main-focus is to feed the *perfect-later* with some hands-on.

The idea is to show how to efficiently rebase/squash commits of a cluttered branch before releasing it to the public (i.e. a non-feature-branch).

[presentation]: https://sm-paul-schuette.github.io/git-fresh-up/

## steps to reproduce
```
git checkout
git rebase -i init
```
Make sure in the opening editor you change all the `pick` commands to
```
p 501a50c Ignores system local files
f 4c5922e
r 379e390 readme
f e095aa8 lunch
p c9bb8c0 Add presentation
f 3b7612b fix link

```
