bkt
===

bkt handles file uploads to S3 and not much else.



USAGE
-----

List all buckets:

    $ bkt ls


List all files in a bucket:

    $ bkt ls BUCKET


Create a new bucket:

    $ bkt create BUCKET


Upload a new file:

    $ bkt put BUCKET /path/to/some/file.tar.gz


Download a file to the current directory:

    $ bkt get BUCKET file.tar.gz


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


If you want to keep your credentials somewhere else, you can use the
special `_eval` options to call another command. For example, to use
GNOME Keyring you might do something like this:


    [auth]
    access_key_eval = gnome-keyring-query get aws_access_key
    secret_key_eval = gnome-keyring-query get aws_secret_key




REQUIREMENTS
------------

* [botocore](https://pypi.python.org/pypi/botocore)
