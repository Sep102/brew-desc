# brew-desc.rb - Searchable descriptions for Homebrew formulas

## What is it?

It's an [external command](https://github.com/mxcl/homebrew/wiki/External-Commands) for [Homebrew](https://github.com/mxcl/homebrew). It provides short descriptions for many Homebrew packages, and I hope to eventually include *all* Homebrew packages. You can also search for packages by description.

## Usage

If you already know the name of a package, and you want to see a bit about it, that's easy:

    telemachus ~ ❯❯ brew desc mutt
    mutt: Mongrel of Mail User Agents (part Elm, Pine, Mush, mh, etc)

If you know the kind of thing you're interested in, but not the name of specific items, that's easy too:

    telemachus brew-desc ❯❯ brew desc -s key-value
    redis: A persistent key-value database with built-in net interface
    kumofs: A scalable and highly available distributed key-value store
    cassandra: Highly scalable, eventually consistent, distributed key-value store

Both `-s` and `--search` are acceptable. Searches are always case insensitive. (Notice that as a Homebrew [external command](https://github.com/mxcl/homebrew/wiki/External-Commands), you invoke the script as `brew desc`.)

## Installation

Download and put the file `brew-desc.rb` anywhere in your `$PATH`. Leave the name as is; Homebrew knows how to find it.

## Contributing

I got these descriptions from the [MacPorts](http://www.macports.org/) ports tree. After that, I edited them slightly to make them briefer. There are still at least 500 or so Homebrew formulas without descriptions here, and no doubt these descriptions could be better in many cases.

Please fork, add descriptions (or edit the ones already here) and send a pull request. Thanks.
