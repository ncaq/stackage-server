stackage-server
===============

[![Build Status](https://travis-ci.org/fpco/stackage-server.svg?branch=master)](https://travis-ci.org/fpco/stackage-server)

Server for stable, curated Haskell package sets

This repo is part of the [Stackage project](https://github.com/fpco/stackage),
and the live server can be viewed at https://www.stackage.org.

Running the server will automatically download an SQLite3 database from S3
containing package metadata and snapshot information.  The SQLite3 database is
generated by the `stackage-server-cron` executable in this repository.

You can run this site with `yesod devel`, e.g.:

    stack --install-ghc install yesod-bin
    yesod devel
