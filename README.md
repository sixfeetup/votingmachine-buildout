# Voting Machine buildout

## Install

Clone the buildout

    $ git clone git@github.com:sixfeetup/votingmachine-buildout.git

Put the proper environment in place

    $ cd votingmachine-buildout
    $ cp profiles/buildout.cfg.tmpl buildout.cfg
    $ vi buildout.cfg
    ... uncomment the line for the envrionment you want to run ...

Then bootstrap

    $ python2.6 bootstrap.py

Now run buildout

    $ bin/buildout

## Start up

The buildout includes supervisor, you can start up the whole app
like this

    $ bin/supervisord

Now you can access the site at the http://localhost:51105

### Debug start up

If you want to use pdb or any other interactive commands you can do
the following.

    $ bin/supervisorctl stop paster
    $ bin/paster serve etc/paster.ini --reload

This will start the program up in the foreground.
