# -*- mode: ruby -*-
# vi: set ft=ruby :
# BASADO EN: https://ostechnix.com/install-mongodb-using-vagrant-in-linux/
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.box_check_update = false
  config.vm.define "MongoDB5"
  config.vm.network "public_network"
  config.vm.provision "shell", path: "mongo-bootstrap.sh"
  config.vm.provider "virtualbox" do |v|
    v.memory = 2048
    v.cpus = 2
    v.name = "MongoDB-5"
  end
end
