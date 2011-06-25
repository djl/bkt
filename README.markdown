bkt
===

bkt handles file uploads to S3 and not much else.



USAGE
-----

List all buckets:

    bkt buckets


List all files in a bucket:

    bkt ls BUCKET_NAME


Upload a new file:

    bkt put BUCKET_NAME /path/to/some/file.tar.gz


Delete a file:

    $ bkt rm BUCKET_NAME file.tar.gz



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
