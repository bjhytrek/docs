# MoFed style standards

## Use 4 spaces, not tabs or 2 spaces.
- Use soft tabs
- use 4 spaces for tab
- Atom space clean plugin: [tabs-to-spaces](https://atom.io/packages/tabs-to-spaces)


## When tagging a version:
- Don't use `v`
- use semver
  - Breaking.minor.hotfix
- start with 1.0.0-alpha.1
  - iterate the alpha.# for alpha iterations
- when making an update always use alpha until it is ready to realease
- when it is ready for realease drop the -alpha.# for the stable release.

## For strings in js
- use the \` not ' or "

## Let and Const
- Var is dead to us.
- Const is used most of the time.
- only use let if you need to mutate a variable, not typically needed.

## Write pure functions
