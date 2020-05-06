# Ansible Role for etcd

## 4.4.0 - TBC

### Major Changes

  - Support Fedora 31
  - Support Debian 10
  - Template complex variable with Jinja `namespace()`
  - Replace use of `ansible_hostname` with `inventory_hostname`
  - `molecule -s default` with delegated to localhost

## 4.3.0 - 2020-04-22

### Major Changes

  - Template `molecule -s default` with dummy docker driver
  - Support CentOS/RHEL 8
  - Support Ubuntu 20.04
  - Remove Ubuntu 16.04 support
  - Upgrade minimal Molecule support to 3.0.2
  - Migrate role name to lowercase or underline
  - Migrate group name to lowercase or underline
  - Migrate molecule `group_vars` to file
  - Download archives to `{{ ansible_user_dir }}/.ansible/tmp`

## 4.2.0 - 2020-02-13

### Major Changes

  - Migrate molecule driver to Libvirt
  - Migrate molecule verifier to Ansible
  - Support Ubuntu 19.10

## 4.1.0 - 2020-01-16

### Major Changes

  - Default `interpreter_python` with `python3`
  - Bugfix `python3-xml` not exists for openSUSE Leap 15.1

## 4.0.0 - 2019-11-05

### Major Changes

  - Upgrade minimal Ansible support to 2.9.0
  - Upgrade Travis CI test as Ubuntu Bionic based

## 3.5.0 - 2019-10-06

### Major Changes

  - Support openSUSE Leap 15.1
  - Default with Python 3
  - Revamp molecule test with vagrant

## 3.4.0 - 2019-09-18

### Major Changes

  - Run molecule test manually on Travis CI

## 3.3.0 - 2019-08-27

### Major Changes

  - Update for RHEL 7
  - Add Vagrant test for RHEL 7
  - Download archives to `/var/cache/ansible`
  - Upgrade packages if archives not found from `/var/cache/ansible`
  - Restart service serially

## 3.2.0 - 2019-07-08

### Major Changes

  - Update LXD test profile for Kubernetes v1.15.0 support
  - Add dummy tasks and vars placeholder for multi OS support
  - Fix molecule `group_vars` with links
  - Replace `with_items` with `loop`
  - Replace `with_dict` with `var`
  - Replace `with_first_found` with `lookup('first_found')`
  - Update Vagrant test with `private_network`
  - Reduce hardcoded `ansible_default_ipv4`

## 3.1.0 - 2019-06-13

### Major Changes

  - Always include default variables from `vars/main.yml`
  - Always use `become: true` with molecule, especially for vagrant
  - Abstract archive download checksum with multiple version support
  - Improve service restart implementation
  - Revamp multi node test with vagrant
  - Replace `inventory_hostname` with `ansible_hostname`

## 3.0.0 - 2019-05-20

### Major Changes

  - Upgrade minimal Ansible support to 2.8.0
  - Improve handlers implementation
  - Restart service if templates changed
  - Enable TLS protocol
  - Support certificates path customization
  - Simplify service owner as root, simpler Kubernetes intergration

## 2.6.0 - 2019-05-04

### Major Changes

  - Refine Travis CI Molecue test cases

## 2.5.0 - 2019-04-17

### Major Changes

  - Pre-download archives with checksum
  - Run test with `travis_wait 120`

## 2.4.0 - 2019-03-03

### Major Changes

  - Run systemd service with specific system user
  - Add multi-node support
  - Add openSUSE Leap 15 support

## 2.3.0 - 2019-01-30

### Major Changes

  - Porting test to Molecule based
  - Add python-etcd3 for Ansible etcd3 support

## 2.2.0 - 2019-01-26

  - Initial release for Ansible 2.6 or higher
  - Support both Ubuntu 16.04/18.04 and RHEL/CentOS 7
