# A Virtual Machine for Ruby on Rails

## Introduction

This project automates the setup of a development environment for creating a default frontend for Ruby on Rails itself. Using Vagrant and Virtualbox, simply "vagrant up" and begin editing your Rails Apps for a deployment.

Core Deployment options available in ./Vagrantfile

## Requirements

* [VirtualBox](https://www.virtualbox.org)

* [Vagrant](http://vagrantup.com)

* [MobaXterm](http://mobaxterm.mobatek.net/)
  - Recommended Windows install SSH

## How To Build The Virtual Machine - Linux

    host $ git clone https://github.com/fp-programming/ruby-on-rails-vagrant.git
    host $ cd ruby-on-rails-vagrant
    host $ vagrant up

## How To Build The Virtual Machine - Windows

    Download/Clone the Git repository fp-programming/ruby-on-rails-vagrant
    Cmd$ cd X:\<ruby-on-rails-vagrant>\
    Cmd$ vagrant up

## After Installation SSH - Linux

    host $ vagrant ssh
    Welcome to Ubuntu 14.04.2 LTS (GNU/Linux 3.13.0-55-generic x86_64)
    ...
    vagrant@rails-dev-box:~$


## After Installation SSH - Windows

MobaXterm
* Create new SSH Session
  - Type: SSH
  - Host: 127.0.0.1
  - User: Vagrant
  - Port: 2222
* Advanced SSH Settings
  - Uncheck All Settings
  - Check "Use Private Key" - X:\<ruby-on-rails-vagrant>\.vagrant\machines\default\private_key

## Editing and Creation

### Prior to deployment
Update setup-env.sh file with any local environment setting you want to be sourced.
### Deployment
Any updates you make will automatically be updated on your rails website once it
has been saved to your local machine. If you wish to use any of the rails templates
SSH into the virtualbox.

### Example:
    $ cd /vagrant
    $ rails generate controller NewController


## Ruby Website

    Open Chrome or other browser
    [Welcome Aboard](http://10.0.32.1:3000)

## Optional Development Tools

* Development tools

* Git

* Ruby 2.3

* Bundler

* SQLite3, MySQL, and Postgres

* Databases and users needed to run the Active Record test suite

* System dependencies for nokogiri, sqlite3, mysql, mysql2, and pg

* Memcached

* Redis

* RabbitMQ

* An ExecJS runtime

## Citations
Ruby On Rails Vagrant was produced using the Rails Dev Box located [here](https://github.com/rails/rails-dev-box)
* Slimmed down deployment for Ruby On Rails frontend
* Updated to use systemd

## License

Released under the MIT License, Copyright (c) 2012–<i>ω</i> Xavier Noria.
