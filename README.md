# FedEx Voting buildout

Clone the buildout

    $ git clone git@github.com:sixfeetup/fedexvoting-buildout.git

Then bootstrap (the `-v` is to avoid a buildout bug)

    $ cd fedexvoting-buildout
    $ python2.6 bootstrap -v 1.4.2

Now run buildout

    $ bin/buildout

Now you can start up the instance like this for development

    $ bin/paster server src/fedexvoting/development.ini --reload
