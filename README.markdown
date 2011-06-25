bkt
===

bkt handles file uploads to S3 and not much else.



USAGE
-----

List all buckets:

    $ bkt buckets
    home_backups
    project_backups
    work_backups


List all files in a bucket:

    $ bkt ls home_backups
    documents-20110410.tar.gz.gpg
    ...


Upload a new file:

    $ bkt put home_backups some_file.txt


Delete a file:

    $ bkt rm home_backups some_file.txt



SETUP
-----

Create an ini file `~/.bkt` and give it your access and secret
keys in an `auth` section:

    [auth]
    access_key = 1234567890asdf
    secret_key = LOLSECRETS



REQUIREMENTS
------------

* [boto](http://boto.cloudhackers.com/)



TODO
----

* (Explicit) creation and deletion of buckets
* Set/modify permissions for whole buckets or individual files
* Documentation
* Deletes
