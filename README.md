# Periodic Programming Exercises

This is an "almost" monorepo to record programming exercises by programming language and problem. Problems will come from online, books, interviews or just things I dream up.
Since this is skill building for myself on no particular timetable, I don't want to over structure it (yet).


The directory layout is:

```bash
$ tree -CF ${GIT_ROOT:-.} 
.
├── bin/
├── by-language/
│   ├── clojure/
│   │   └── problems/
│   │       └── start/
│   │           ├── bin/
│   │           ├── doc/
│   │           └── src/
│   │               └── test/
│   ├── go/
│   │   └── problems/
│   │       └── start/
│   │           ├── bin/
│   │           ├── doc/
│   │           └── src/
│   │               └── test/
│   ├── julia/
│   │   └── problems/
│   │       └── start/
│   │           ├── bin/
│   │           ├── doc/
│   │           └── src/
│   │               └── test/
│   ├── python3/
│   │   └── problems/
│   │       └── start/
│   │           ├── bin/
│   │           ├── doc/
│   │           └── src/
│   │               └── test/
│   ├── rust/
│   │   └── problems/
│   │       └── start/
│   │           ├── bin/
│   │           ├── doc/
│   │           └── src/
│   │               └── test/
│   ├── scala/
│   │   └── problems/
│   │       └── start/
│   │           ├── bin/
│   │           ├── doc/
│   │           └── src/
│   │               └── test/
│   └── typesscript/
│       └── problems/
│           └── start/
│               ├── bin/
│               ├── doc/
│               └── src/
│                   └── test/
├── doc/
├── README.md  # you are here
```


Created with:

```bash
# Add the programming languages you want. Assumes each language has the same layout, which isn't true.
# Note that `start` is the "starting" point for a problem solution. There may be other (better) ways to create
#   a starting point, e.g. for python `poetry new`. This will evolve.
mkdir -p bin doc by-language/{python3,typesscript,rust,clojure,go,scala,julia}/problems/start/{bin,doc,src/test}

# Install hub. Simplies github interaction.
$ sudo snap install hub
$ snap info hub
name:      hub
summary:   hub is a command-line wrapper for git that makes you better at GitHub.
publisher: Ricardo N Feliciano (felicianotech)
contact:   https://Feliciano.Tech/contact
license:   unset
description: |
  As a contributor to open-source
  
  Whether you are beginner or an experienced contributor to open-source, hub makes it easier to
  fetch repositories, navigate project pages, fork repos and even submit pull requests, all from the
  command-line.
  
  As an open-source maintainer
  
  Maintaining a project is easier when you can easily fetch from other forks, review pull requests
  and cherry-pick URLs. You can even create a new repo for your next thing.
  
  Using GitHub for work
  
  Save time at work by opening pull requests for code reviews and pushing to multiple remotes at
  once. Even GitHub Enterprise is supported.
  
  Hub is made by GitHub. This snap is packaged by Ricardo N Feliciano (FelicianoTech) using the
  `hub` source code available by GitHub.
commands:
  - hub
snap-id:      oaQHXl9Nl2aedf7khkmFg2dyi299y9U0
tracking:     stable
refresh-date: yesterday at 23:07 EDT
channels:
  stable:    v2.12.1 2019-06-30 (19) 12MB classic
  candidate: ↑                            
  beta:      ↑                            
  edge:      0       2017-05-17  (1) 34MB -
installed:   v2.12.1            (19) 12MB classic

$ git init .; git add *; git commit -m 'start'; hub create; git push

```
