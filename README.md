# clj-user-deps

My user deps.edn file for Clojure's clj and clojure CLI tooling.

Nothing interesting to see for anyone else, probably.

This is mostly inspired by the one found in [seancorfield/dot-clojure](https://github.com/seancorfield/dot-clojure) and is quite the similar in many ways, but the dot-clojure one is a way more better example altogether (thanks!).


## Notes about the Usage

User deps.edn file is most often stored in $HOME/.clojure/, I assume. However, I currently have this deps.edn located inside a "normal" project directory and therefore I use an environment variable to point my clj/clojure tools to the right file:

```
$ export CLJ_CONFIG=/path/to/the/containing/directory
```

Currently there are only a couple of aliases defined in the file. For example the alias named as cider-nrepl can be invoked like this:

```
    $ clj -A:cider-nrepl
```
If the aforementioned command was successful, there should now be an nrepl waiting for [CIDER](https://github.com/clojure-emacs/cider) connection in the port number 60607. The port numbers are hardcoded in. 
