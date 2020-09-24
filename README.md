# SSH Key based User Management using Ansible

This reporsiotry includes Ansible playbook for managing users and their SSH Key based authentication.

## What this playbook does?

* Each user will have a set of SSH keys
* Each user will be given their private key for login.
* Each user will belong to a group named TAC.
* All users in TAC group will be restricted to perform limited commands & functions.
* No user will be allowed to switch to root user.
* Users will not be allowed to edit sudoers file as well.


## Usage

```bash
$ git clone https://github.com/amans118/User-Management.git
$ cd User-Management
$ ansible-playbook user_management.yml -u username --ask-pass
```

#### Important:
*This playbook is tested on Ubuntu/Debian based systems only.*:
