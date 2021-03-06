nagios-cli
==========

About
-----

nagios-cli is a Nagios command line interface, exposing some features that are
available via the web based graphical user interface.


Requirements
------------

Required:

*  Nagios 2.x or 3.x
*  Python 2.4+

Optional:

*  libreadline


Usage
-----

The default configuration will look for the `status_file` file in the
`/var/log/nagios/status.dat` file, and it expects the `command_file` to be
available at `/var/log/nagios/rw/nagios.cmd`. If you wish to override
this, you can generate a configuration file with:

    nagios-cli -c nagios-cli.cfg --write

To specify a location to an alternative configuration file, use:

    nagios-cli -c <filename>

To see all available options, use:

    nagios-cli --help

