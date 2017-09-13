# ansible-role-vagrant-java-dev [![Build Status][travis.svg]][travis]

An Ansible role for a Vagrant-based Java/Scala development setup.

Available on Ansible Galaxy at [`naftulikay.vagrant-java-dev`][galaxy].

## Requirements

A Vagrant machine running a supported operating system.

## Role Variables

<dl>
  <dt><code>vagrant_user</code></dt>
  <dd>The username of the Vagrant user, defaults to <code>vagrant</code></dd>
</dl>

> Please see the upstream [`naftulikay.vagrant-base`][vagrant-base] and [`naftulikay.java-dev`][java-dev] roles for
additional supported variables.

## Dependencies

 - [`naftulikay.vagrant-base`][vagrant-base]: Provides base Vagrant configuration.
 - [`naftulikay.java-dev`][java-dev]: Provides a basic Java development environment.

## Example Playbook

Install a Java development environment within the Vagrant machine:

```
---
- hosts: all
  roles:
    - role: vagrant-javas-dev
```

## LICENSE

MIT.

 [travis]: https://travis-ci.org/naftulikay/ansible-role-vagrant-java-dev
 [travis.svg]: https://travis-ci.org/naftulikay/ansible-role-vagrant-java-dev.svg?branch=master
 [galaxy]: https://galaxy.ansible.com/naftulikay/vagrant-java-dev/
 [vagrant-base]: https://galaxy.ansible.com/naftulikay/vagrant-base/
 [java-dev]: https://galaxy.ansible.com/naftulikay/java-dev/
