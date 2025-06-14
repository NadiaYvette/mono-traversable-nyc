# Fork of mono-traversable

Michael Snoyman deserves all the credit. I'm just maintaining a fork for
the sake of including some PRs that haven't had time to get looked after
in a great while. conduit and such have some back-dependencies to the
original that would take a fork of that to point back to. The fork was
largely for the sake of mono-traversable, so the other packages in the
repo haven't been as heavily modified.

I left the copyrights as-is basically for giving Snoyman all of the
credit, and hopefully none of the blame.

## mono-traversable mega-repo

[![Tests](https://github.com/NadiaYvette/mono-traversable-nyc/actions/workflows/tests.yml/badge.svg)](https://github.com/NadiaYvette/mono-traversable-nyc/actions/workflows/tests.yml)

This repository contains packages in the mono-traversable and classy-prelude
families. Please see the individual READMEs for more details:

You probably want to view [the README for mono-traversable
itself](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/mono-traversable#readme).

Additional packages in this repository:

* [mono-traversable](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/mono-traversable#readme)
  providing a set of classes for dealing with monomorphic data structures (like `ByteString` and `Text`)
  in a similar way to how the standard libraries treat polymorphic structures like lists
    * [mono-traversable-instances](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/mono-traversable-instances#readme),
      containing orphans instances for mono-traversable classes
* [chunked-data](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/chunked-data#readme),
  providing typeclasses for dealing with various chunked data representations
* [mutable-containers](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/mutable-containers#readme),
  abstractions and concrete implementations of mutable containers
* [conduit-combinators](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/conduit-combinators#readme),
  commonly used conduit functions, for both chunked and unchunked data
* [classy-prelude](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/classy-prelude#readme),
  a Prelude replacement based around the above packages (and many others)
    * [classy-prelude-conduit](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/classy-prelude-conduit#readme),
      extends classy-prelude with [conduit support](https://github.com/snoyberg/conduit)
    * [classy-prelude-yesod](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/classy-prelude-yesod#readme),
      extends classy-prelude-conduit with [Yesod web framework support](http://www.yesodweb.com)
* [minlen](https://github.com/NadiaYvette/mono-traversable-nyc/tree/master/minlen#readme),
  provided a newtype wrapper with type-level annotation of minimum container
  length. This is a generalization of the `Data.NonNull` module in `mono-traversable`
