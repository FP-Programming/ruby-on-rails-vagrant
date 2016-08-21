# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure('2') do |config|
  config.vm.box      = 'ubuntu/wily64'
  config.vm.hostname = 'rails-dev-box'

  config.vm.network "private_network", ip:"10.0.32.1"

  config.vm.provision :shell, path: 'bootstrap.sh', keep_color: true

  config.vm.provider 'virtualbox' do |v|
    v.memory = 1024
  end
end
