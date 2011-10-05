Supervisord-Nagios-Plugin
-------------------------

Instalation
-----------

Copy the file check_supv.py to your Nagios/Icinga directory and make executable 


Configuration
-------------
Set the supervisorctl status command, default is

::

        SUPERV_STAT_CHECK='sudo supervisorctl status'

Please make sure nagios/icinga user can run the command without password

Command
-------
Run the command with the name of the supervisord process as it appears in ``supervisorctl status``

::

        check_supv -p PROCESS_NAME

