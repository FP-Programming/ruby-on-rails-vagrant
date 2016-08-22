# A Virtual Machine for Ruby on Rails
For educational and entertainment purposes only. There are some other, fancier deployment options such as [railsbox](http://railsbox.io) if you know what you're doing, but this will help get you through the [Rails Tutorial](https://www.railstutorial.org/book) with a proven environment that doesn't require a lot of knowledge in Linux to set up.

## Introduction

This project automates the setup of a development environment for creating a default frontend for Ruby on Rails itself. Using Vagrant and Virtualbox, simply "vagrant up" and begin editing your Rails Apps for a deployment.

Core Deployment options available in ./Vagrantfile

## Requirements

* [git](https://git-scm.com/downloads)

* [VirtualBox](https://www.virtualbox.org)

* [Vagrant](http://vagrantup.com)


## How To Build The Virtual Machine
If you are using Windows, it is best to use GIT Bash for all terminal commands

    host $ git clone https://github.com/Finite-Programming/ruby-on-rails-vagrant.git
    host $ cd /path/to/install/ruby-on-rails-vagrant
    host $ vagrant up

## After Installation SSH

    host $ vagrant ssh
    Welcome to Ubuntu 14.04.2 LTS (GNU/Linux 3.13.0-55-generic x86_64)
    ...
    vagrant@rails-dev-box:~$


## Editing and Creation

### Prior to deployment
Update setup-env.sh file with any local environment setting you want to be sourced.

### Deployment
Any updates you make will automatically be updated on your rails website once it
has been saved to your local machine. If you wish to use any of the rails templates
SSH into the virtualbox.

#### Example:
    $ cd /vagrant
    $ rails generate controller NewController

## Ruby Website

    Open Chrome or other browser
    [Welcome Aboard](http://10.0.32.1:3000)

## More on Deployment
Ruby On Rails Vagrant deploys a new rails template for 5.0.0.1. If you need a different
rails deployment follow these steps.

    * Run 'vagrant up' from your platform of choice
    * Delete all but the core files from your /vagrant environment. Core Files:
      - .vagrant
      - bootstrap.sh
      - MIT-LICENSE
      - README.md
      - Vagrantfile
    * SSH into your virtual machine and run the new rails command
      - $ rails _X.x.x.x_ new 'myapp'

## Required Development Tools

* Ruby 2.3

* Rails 5.0.0.1

* SQLite3

* Nodejs

* System dependencies for nokogiri, sqlite3

* An ExecJS runtime


## Optional Development Tools

* Development tools

* Git

* Bundler

* MySQL, and Postgres

* Databases and users needed to run the Active Record test suite

* System dependencies for mysql, mysql2, and pg

* Memcached

* Redis

* RabbitMQ

## Citations
Ruby On Rails Vagrant was produced using the Rails Dev Box located [here](https://github.com/rails/rails-dev-box)
* Slimmed down deployment for Ruby On Rails requirements
* Added functions to start Ruby on Rails using systemd
* Added a "new" rails template for 5.0.0.1

## License

Released under the MIT License, Copyright (c) 2012–<i>ω</i> Xavier Noria.
