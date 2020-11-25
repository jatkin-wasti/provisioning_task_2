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
- Exit the virtual machine with `exit`
- cd into the tests folder and run `rake spec` to see all of the tests passing!

## Writing the provision file
- First we've imported the public key for the desired version of mongodb and
created a source list file for it
- Then we've updated the package list to include this old version
- We've installed the old version of mongodb, enabled, and started it so that
we have it up and running
- Finally we edit the config file with the sed command to listen to 0.0.0.0
instead of the default location
