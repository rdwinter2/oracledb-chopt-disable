Disable Oracle database options via chopt
=============

## Description

Diable unneeded Oracle database options by removing them from the kernel using chopt.

Options that can be disabled in Oracle 12.2.

* Oracle Advanced Analytics
* Oracle OLAP
* Oracle Partitioning
* Oracle Real Application Testing

This operation is best performed before a database is created.

## Documentation

## Requirements

## Dependencies

None

## Setup

## Testing

## Role Variables

| Name | Default Value | Description |
|------|---------------|-------------|
|

## Example Playbook

```{.yml}
- name: Exercise the role oracledb-chopt-disable
  hosts: all
  become: true
  become_method: 'sudo'
  roles:
    - { role: oracledb-chopt-disable }
```

## Configuration

## Road Map

### Planned Additions

### Current Issues

### Changelog

## Discussion

## Transcluded Content

## License

MIT

## Author Information

| Author                | E-mail               |
|-----------------------|----------------------|
| Robert D. Winter, 2nd |  rdwinter2@gmail.com |

## References

* [Chopt Tool](https://docs.oracle.com/en/database/oracle/oracle-database/12.2/ladbi/chopt-tool.html#GUID-057E4EFC-74ED-43B3-B03B-C83C5A5D3C7F)
* [How to Check and Enable/Disable Oracle Binary Options (Doc ID 948061.1)](https://support.oracle.com/epmos/faces/DocumentDisplay?_afrLoop=385003149009500&id=948061.1+&_afrWindowMode=0&_adf.ctrl-state=i3eqxakzs_4)