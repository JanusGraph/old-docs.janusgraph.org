# docs.janusgraph.org

[![Website][website-shield]][website-link]

[website-shield]: https://img.shields.io/website-up-down-green-red/http/docs.janusgraph.org.svg?label=docs.janusgraph.org
[website-link]: http://docs.janusgraph.org

This repository contains the _generated_ documentation which is served on
http://docs.janusgraph.org . To update the documentation for a particular
version of JanusGraph, do not send a PR manually updating HTML files, because
those changes will be overwritten in the next docs update.

Instead, please do the following:

* modify the source AsciiDoc files in
  [`janusgraph/docs`](https://github.com/janusgraph/janusgraph/tree/master/docs)
* build the docs using
  [`janusgraph/docs/build-and-copy-docs.sh`](https://github.com/JanusGraph/janusgraph/blob/master/docs/build-and-copy-docs.sh)
  and then create a PR using the output files from this script
