ruby
=========

Ansible role for downloading Ruby source archives to the control server, then extracting them to the target host.

Role Variables
--------------
Set the ```ruby_version``` parameter to install other versions of Ruby

        ruby_version: 2.3.1
        
Available versions:

    2.1.10
    2.2.5
    2.3.1

Set the ```prefix``` parameter to install somewhere other than ```opt/ruby```

        prefix: "opt/ruby"

Set the ```compile``` parameter to ```yes``` to compile Ruby from source

        compile: no
        
License
-------

MIT

Testing
-------
Run the following command:

        ansible-playbook ruby/tests/test.yml

