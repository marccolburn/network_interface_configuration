Network Interface Configuration
=========

Configure network interfaces for IOS, IOSXR, JUNOS, EOS, and Cumulus Linux.

Requirements
------------


Role Variables
--------------
physical_interfaces: List of Dictionaries containing physical interfaces and info.
* name: Name of the interface
* description: Interface description
* enabled: Turn the interface on or off

logical_interfaces: List of dictionaries containing physical interfaces and info.
* name: Name of interface
* ipv4: Dictionary containing info on ipv4 parameters of interface
  * address: IPv4 address and mask

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: network_interface_configuration }

License
-------

BSD

Author Information
------------------

Marc Colburn Red Hat
