# Ansible_Documentation
Links to all the docs referenced for writing ansible modules

## Overview
Ansible documentation is annoying.  This page will include lots of links to the useful bits if info needed to develop an ansible module.
- [Module Development](https://docs.ansible.com/ansible/latest/dev_guide/developing_modules_general.html)
- [Getting Started with Template Code](https://docs.ansible.com/ansible/latest/dev_guide/developing_modules_general.html)

## Developing a Module
### Dev Environment
Here are some useful tips for being able set up your dev environment so you can test out all the features of your role

#### Ansible Configuration
While writing the documentation, since the role is not installed "properly" testing out things like `ansible-doc` can be difficult.  Create a file called `ansible.cfg` (or one of the other methods described in the ansible doc config info) to set the settings below.

```
[defaults]
library = ./
module_utils = ./module_utils
doc_fragment_plugins = ./plugins/doc_fragments
```

- [Ansible Configuration](https://docs.ansible.com/ansible/latest/reference_appendices/config.html)

#### Python Modules
- ansible
- ansible-lint
- molecule
- docker

### Developing a Module in a Role
The documentation for the directory layout for your role so that it can include a Module.
- [Directory Layout for Modules](https://docs.ansible.com/ansible/2.9/user_guide/playbooks_reuse_roles.html#embedding-modules-and-plugins-in-roles)

### Developing a Module in a Collection
- Pathing in collections is annoying.  Once you figure it out it's not a big deal.  Ansible is looking for a directory called `ansible_collections` as the root of the collection.  Make sure your collection is in there and it will all be good.

## Module Utilities
This has information about creating common/reusable python modules for your code.  Also has information about using module utilities already included with Ansible for use in developing your own modules.

- [Module Utilities](https://docs.ansible.com/ansible/latest/dev_guide/developing_module_utilities.html)
- [Source Code from Github](https://github.com/ansible/ansible/tree/devel/lib/ansible/module_utils)
- [Reference Manual](https://docs.ansible.com/ansible/latest/reference_appendices/module_utils.html)

The last link is basically from the github page, just a tad easier to read.

## Module Documentation
- [Module Documentation Guide](https://docs.ansible.com/ansible/2.9/dev_guide/developing_modules_documenting.html)


## Debugging Ansible
The key to remember is you are essentially "compiling" the ansible code into a zip file, then you run the zip file with python.  Python will invoke the PDB trace you insert and you can see what's going on from there.
- [Debugging](https://docs.ansible.com/ansible/latest/dev_guide/debugging.html)



[]()
[]()


## Testing

### Testing with PyTest


### Testing with Molecule
Molecule is the official testing platform for Ansible.
- [Molecule Documentation](https://molecule.readthedocs.io/en/latest/)

## Linting
