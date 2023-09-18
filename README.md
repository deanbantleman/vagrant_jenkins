# Overview

This code will spin up a CENTOS 7 server with Hashicorp Vagrant. It will then install Jenkins and configure Jenkins using an Ansible playbook.

# Environment

This code was executed on a Windows 10 machine and the Windows Subsystem for Linux (WSL) was used to host an Ubuntu 20.04.6 execution environment.

Ansible needs to be installed on the Ubuntu host.

# Prerequisites

1) Configure Vagrant to run in WSL by following this link: [https://blog.thenets.org/how-to-run-vagrant-on-wsl-2/]

2) Install Ansible with the following commands:

   ```
   sudo add-apt-repository --yes --update ppa:ansible/ansible
   sudo apt install ansible
   ```
# Running the code

1) Change directory into the Vagrant project directory, replacing %username% with your windows username:

   ```
   cd /mnt/c/Users/%username%/projects
   ```
2) Clone this repository:

   ```
   git clone git@github.com:deanbantleman/vagrant_jenkins.git
   ```

3) Change directory into the code directory:

   ```
   cd vagrant_jenkins
   ```

4) Run Vagrant:

   ```
   vagrant up
   ```

# Re-run provisioning

If your instance is already running or you need to re-run your ansible code you can run the command:

```
vagrant provision
```

   



