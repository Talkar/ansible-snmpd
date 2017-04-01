# Ansible Role: snmpd

## Description

Ansible role for installing and configuring SNMP v3 on RHEL/CentOS/Fedora/OpenSUSE/Debian/Ubuntu/ArchLinux.

## Installation

```
$ git clone https://github.com/inperfo/ansible-snmpd.git

```

## Role Variables

| Variable             | Default         | Comments (type)                                   |
| :---                 | :---            | :---                                              |
| snmp_version         | 3               | Default SNMP Version                              |
| snmp_user            | snmp            | SNMP User                                         |
| snmp_sec_level       | authPriv        | SNMP Access Mode                                  |
| snmp_auth_protocol   | SHA             | SNMP Authentication Protocol                      |
| snmp_priv_protocol   | AES             | SNMP Encryption Protocol                          |

## Example Playbook

```yml
- hosts: all
  roles:
     - snmpd
```

After adding your hosts to inventory.ini just run ansible-playbook:

```
$ ansible-playbook snmpd.yml

```

## Author

* [Alexander Nesterov](https://www.facebook.com/nester.wsx)
 
## License

None. 

## Copyright

(c) Alexander Nesterov
