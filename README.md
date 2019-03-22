# docs.janusgraph.org

[![Website][website-shield]][website-link]

[website-shield]: https://img.shields.io/website-up-down-green-red/https/docs.janusgraph.org.svg?label=docs.janusgraph.org
[website-link]: https://docs.janusgraph.org

This repository contains the _generated_ documentation which is served on
https://docs.janusgraph.org . To update the documentation for a particular
version of JanusGraph, do not send a PR manually updating HTML files, because
those changes will be overwritten in the next docs update.

Instead, please do the following:

1. modify the source AsciiDoc files in
   [`janusgraph/docs`](https://github.com/janusgraph/janusgraph/tree/master/docs)
1. build the docs using
   [`janusgraph/docs/build-and-copy-docs.sh`](https://github.com/JanusGraph/janusgraph/blob/master/docs/build-and-copy-docs.sh)
1. preview the output files from the script above locally in your browser to
   verify that everything looks as expected
1. create a feature branch with these files to be used for your PR
1. also create a `gh-pages` branch to point to the same commit as your feature
   branch for the preview site
1. publish a [preview of your changes on
   GitHub](https://github.com/JanusGraph/janusgraph.org/blob/master/README.md#preview-via-github),
   making appropriate substitutions in the instructions, i.e,
   `s/janusgraph.org/docs.janusgraph.org/g`, so that others can preview it
   easily by pushing the `gh-pages` branch with your HTML pages to your fork
1. create a PR using your **feature branch** and link to your preview site so
   that others can see the changes without having to rebuild your PR manually
