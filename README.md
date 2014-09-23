Spamassassin
============

Perform install and basic configuration of Spamassassin including SPF and DKIM
support.

This role is still in the early stages.

Requirements
------------

For RedHat family systems a repository with perl-Mail-SPF and perl-Mail-DKIM
available needs to be configured before running this role - EPEL can be used
for that purpose.

Role Variables
--------------

spamassassin_lock_method_flock_enable: true
spamassassin_disable_spf: false
spamassassin_disable_dkim: false

Dependencies
------------

N/A

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: mxs
      roles:
         - { role: goetzk.spamassassin, spamassassin_disable_spf: true }

License
-------

GPL2+

Author Information
------------------

Issues or feedback can be reported to the author at karl@kgoetz.id.au; please
prefix the subject with 'ansible' or 'role'.

