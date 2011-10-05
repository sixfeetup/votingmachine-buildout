# FedEx Voting buildout

Clone the buildout

    $ git clone git@github.com:sixfeetup/fedexvoting-buildout.git

Then bootstrap

    $ cd fedexvoting-buildout
    $ python2.6 bootstrap.py

Now run buildout

    $ bin/buildout

Now you can start up the instance like this for development

    $ bin/paster server src/fedexvoting/development.ini --reload
