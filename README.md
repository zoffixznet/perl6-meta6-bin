# META6-bin
[![Build Status](https://travis-ci.org/gfldex/perl6-meta6-bin.svg?branch=master)](https://travis-ci.org/gfldex/perl6-meta6-bin)

Create and check META6.json files and module skeletons.

Depends on `git` and `curl` in `$PATH` and got a timeout of 60s for each call
to both. Those are used to setup a git and github repo.

Module skeletons include basic directories, `META6.json`, `t/meta.t`,
`.travis.yml` and a `README.md`. The latter includes a link to
[travis-ci](https://travis-ci.org/).

# SYNOPSIS

    meta6 --create --name=<project-name-here> --force
    meta6 --check
    meta6 --create-cfg-dir
    meta6 --new-module --name=<Module::Name::Here> --force --skip-git --skip-github

# General Options

    --meta6-file=<path-to-META6.json> # defaults to ./META6.json

# Create Options

    --name
    --description
    --version # defaults to 0.0.1
    --perl # defaults to 6.c
    --author # defaults to user/name from ~/.gitconfig
    --auth # defaults to credentials/username from ~/.gitconfig

