# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "Kals/Fox"

  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.network "private_network", ip: "192.168.33.10"

  # config.vm.network "public_network"
  
  config.vm.hostname = "fox"

  config.vm.synced_folder "E:/Fox/Code", "/home/vagrant/www"

  config.vm.provider "virtualbox" do |vb|
    vb.name = "fox"
    vb.memory = "512"
  end

  # config.push.define "atlas" do |push|
  #   push.app = "YOUR_ATLAS_USERNAME/YOUR_APPLICATION_NAME"
  # end

end
