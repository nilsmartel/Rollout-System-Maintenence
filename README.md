# Rollout

Tool for system maintenance.

Ensure that a set of files (binaries, configurations, text)
are present on a sytem and held up to date with respect to sources like git
or derived from other files

## How it works:

you write an `.ensure` file, with several steps in it.
A step might

- ensure that a git repo is cloned to a specific location on your system.
- a binary is installed
- a command is executed and the result is held up to date with respect to changing input

A step has a way of checking, wether it's inputs changed and, should that be the case, refreshes it's output.
