# Ansible Role for etcd

## 3.2.0 - TBC

### Major Changes

  - Update LXD test profile for Kubernetes v1.15.0 support
  - Update molecule \>=2.22rc1 for Ansible 2.8.0 support
  - Add dummy tasks and vars placeholder for multi OS support

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
