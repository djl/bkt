bkt
===

bkt handles file uploads to S3 and not much else.



USAGE
-----

List all buckets:

    bkt ls


List all files in a bucket:

    bkt ls BUCKET


Create a new bucket:

    bkt create BUCKET


Upload a new file:

    bkt put BUCKET /path/to/some/file.tar.gz


Delete a file:

    $ bkt rm BUCKET file.tar.gz


Delete a bucket:

    $ bkt rm BUCKET


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

* Tidy up help/error messages (unindent)
* Progress bar for uploads
* Set/modify permissions for whole buckets or individual files
* Documentation
