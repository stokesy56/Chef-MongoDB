# Mongo Cookbook :man_cook: :fried_egg: :carrot: :avocado: :grape:

This is a cookbook for MongoDB

## Summary
We need to create a reusable chef cookbook for installing and managing MongoDB servers.

## Tasks
Add new ChefSpec tests for the following:
- Create a mongod.conf file in /etc/mongod.conf
- Create a mongod.service file in /lib/systemd/system/mongod.service
- MongoDB service should be enabled
- MongoDB service should be started

And InSpec tests for the following:
- MongoDB is running
- MongoDB is enabled
- MongoDB is listening on 27017 by default
- MongoDB is listening on 0.0.0.0 by default

Create a recipe that installs and configures this cookbook correctly to pass all these tests.

Use attributes to allow the port number and ip to be configurable.
