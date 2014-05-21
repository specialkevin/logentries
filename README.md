Role Name
========

This role will ensure that the logentries agent is present and configured on the host.

Requirements
------------

This requires version 1.6 of Ansible. There are no other external dependencies.

Role Variables
--------------

The following role variables can be found in defaults/main.yml. You will need to set these variables when you use the role.

** logentries_account_key **

This is the account key that is associated with your logentries account. You can get this key by going to /Account and then the profile tab.

** logentries_watched_files **

This is a list of log files to have logentries track.

Dependencies
------------

The only dependencies for this role is an active account with logentries. You will need the associated account key for the account.

Example Playbook
-------------------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: specialkevin.logentries, logentries_account_key: th1s-k3y5-15nt-ar3al-acc0unt, logentries_watched_files: ['/var/log/syslog', '/var/log/nginx/error.log'] }

License
-------

BSD

Author Information
------------------

Kevin Harriss (special.kevin@gmail.com)
