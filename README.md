Drop into a just-about-tolerable sqlite shell for use with in-memory sqlite.

Vaguely resembles the shell provided by sqlite3 itself, but this one works with
in-memory sqlite db, and is terrible.

Intended for use in tests, if your principles don't forbid that.  I don't
recommend it for use in production.

To use:

    import sqlite3
    import sqliteshell
    conn = sqlite3.connect(':memory:')
    sqliteshell.shell(conn)

Commands:

* help
* schema
* tables

## Run the tests

There are no tests!
