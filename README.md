couch_tools
===========

Perl based CouchDB tools I use

Setup
-----

in the root directory put a file with something like this:

    # cat .couchdb
    export_dir = ./db
    [dev]
        host = 127.0.0.1
        port = 5984
        user = ADMIN USER
        pass = PASSWORD 

in the DB directory some

    # cat .couchdb
    export_dir = .
    [dev]
        host = 127.0.0.1
        port = 5984
        user = ADMIN USER
        pass = PASSWORD 

run it with:
    
    # bin/couch_dump_views dev/[database name]

load the dumped views with:
    
    # cd db/
    # ./load_views.sh
