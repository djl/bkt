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

    bkt create


Upload a new file:

    bkt put BUCKET_NAME /path/to/some/file.tar.gz


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

* Set/modify permissions for whole buckets or individual files
* Choose which region to create a bucket in
* Documentation
