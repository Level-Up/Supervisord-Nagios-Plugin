Supervisord-Nagios-Plugin
-------------------------

Instalation
-----------

Copy the file check_supv.py to your Nagios/Icinga directory and make executable 


Configuration
-------------
Default configuration is to run the command

::

        sudo supervisorctl status $ARG1$

Please make sure nagios/icinga user can run the command without password

Command
-------
Run the command with the name of the supervisord process as it appears in ``supervisorctl status``

::

        check_supv -p PROCESS_NAME

