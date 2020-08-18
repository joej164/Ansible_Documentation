# Ansible_Documentation
Links to all the docs referenced for writing ansible modules

## Overview
Ansible documentation is annoying.  This page will include lots of links to the useful bits if info needed to develop an ansible module

- [Module Development](https://docs.ansible.com/ansible/latest/dev_guide/developing_modules_general.html)
- [Getting Started with Sample Code](https://docs.ansible.com/ansible/latest/dev_guide/developing_modules_general.html)

## Developing a Module

## Developing a Collection
- Pathing in collections is annoying.  Once you figure it out it's not a big deal.  Ansible is looking for a directory called `ansible_collections` as the root of the collection.  Make sure your collection is in there and it will all be good.

## Module Documentation


## Debugging Ansible
The key to remember is you are essentially "compiling" the ansible code into a zip file, then you run the zip file with python.  Python will invoke the PDB trace you insert and you can see what's going on from there.
- [Debugging](https://docs.ansible.com/ansible/latest/dev_guide/debugging.html)



[]()
[]()


## Testing

### Testing with PyTest


### Testing with Molecule

