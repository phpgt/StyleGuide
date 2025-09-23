# Version control

## Commit messages should be written to a specified shape, to categorise and convey intent

A commit message should take the following form:

```
category: short description of what this commit does when applied

closes #123

More meaningful description. This part is optional, but can be used to provide context to others on why you made this decision, or how to integrate.
```

The first line of a commit message is mandatory, and should describe what applying the commit does. Some examples of good commit messages:

+ `fix: apply margin to user dropdown to avoid logo overlap`
+ `feature: user account deletion`
+ `build: upgrade dependencies`
+ `perf: lazy load product list`
+ `test: user account deletion`

Further information inside a commit message is optional. Any tagged issues should come at the start of the description, used by some version control systems to automatically close/reference issues.

A list of all commit categories:

+ `feature` - a user-facing feature, completed in this commit
+ `fix` - this commit resolves a bug
+ `hotfix` - urgent fix, straight to master, bypassing other merges that might be pending
+ `tweak` - a small, minor adjustment to something that isn't big enough to be categorised
+ `wip` - work in progress, but not ready for release (this is almost definitely never going to be seen in the master branch, only in feature branches)
+ `build` - changes to dependencies or build/make scripts
+ `ci` - continuous integration, deployment, or pipeline configuration
+ `perf` - improve performance without changing behaviour
+ `test` - add or adjust tests
+ `docs` - documentation only
+ `refactor` - reduce code without changing behaviour

This type of commit message is referred to as [conventional commits][conventional-commits].

Try to avoid telling jokes or adding emoji into a commit message `fix: 🔑passwords🔑 are not leaked over http 🎉🎉🎉`. Never show frustration through your commit message: `wip: grrrrr why is rinky dinky API so crap????`

[conventional-commits]: https://www.conventionalcommits.org
