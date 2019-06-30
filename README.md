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

```
