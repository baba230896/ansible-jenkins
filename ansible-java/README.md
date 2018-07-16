# Ansible Role: Java

Installs Java for RedHat/CentOS and Debian/Ubuntu linux servers.

## Best Practice 

Use latest Ansible Version

## Role Variables

Available variables are listed below, along with default values:

    # The defaults provided by this role are specific to each distribution.
    java_packages: []

Set the version/development kit of Java to install, along with any other necessary Java packages. Some other options include are included in the distribution-specific files in this role's 'defaults' folder.

    java_home: ""

If set, the role will set the global environment variable `JAVA_HOME` to this value.

## Example Playbook

    - hosts: servers
      roles:
        - ansible-java
