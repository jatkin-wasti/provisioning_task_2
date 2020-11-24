# Homework task
## Intro
This README explains how you can create a simple VM and run tests to check that
the environment is set up correctly
## Prerequisites
- Git
- Ruby
- Vagrant
- VirtualBox

## Instructions
- Clone this repo
- cd into the folder that contains the Vagrantfile and run `vagrant up`
- The virtual machine should be created so let's enter it with `vagrant ssh`
- Run the following command to edit the mongod configuration file
`sudo nano /etc/mongod.conf`
- Change the bindIP value to 0.0.0.0
- Reload mongodb with the port listening on 0.0.0.0 with
```
sudo service mongod restart
```
- Exit the virtual machine with `exit`
- cd into the tests folder and run `rake spec` to see all of the tests passing!
