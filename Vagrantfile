# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.

  # config.vm.network "forwarded_port", guest: 80, host: 8080
  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"
  # vb.gui = true

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"

config.vm.define "vm0" do |vm0|
    vm0.vm.network "private_network", ip: "192.168.56.100"
    vm0.vm.network "public_network", bridge: "enp4s0"

    vm0.vm.provider "virtualbox" do |vb|
      vb.cpus = 2
      vb.memory = "2048"
    end
    vm0.vm.provision "shell", inline: <<-SHELL
      apt-get update
    SHELL
  end

  config.vm.define "vm1" do |vm1|
    vm1.vm.network "private_network", ip: "192.168.56.101"
    vm1.vm.network "public_network", bridge: "enp4s0"

    vm1.vm.provider "virtualbox" do |vb|
      vb.cpus = 2
      vb.memory = "2048"
    end
    vm1.vm.provision "shell", inline: <<-SHELL
      apt-get update
    SHELL
  end

  config.vm.define "vm2" do |vm2|
    vm2.vm.network "private_network", ip: "192.168.56.102"
    vm2.vm.network "public_network", bridge: "enp4s0"

    vm2.vm.provider "virtualbox" do |vb|
      vb.cpus = 2
      vb.memory = "2048"
    end
    vm2.vm.provision "shell", inline: <<-SHELL
      apt-get update
    SHELL
  end

  config.vm.define "vm3" do |vm3|
    vm3.vm.network "private_network", ip: "192.168.56.103"
    vm3.vm.network "public_network", bridge: "enp4s0"

    vm3.vm.provider "virtualbox" do |vb|
      vb.cpus = 2
      vb.memory = "2048"
    end
    vm3.vm.provision "shell", inline: <<-SHELL
      apt-get update
    SHELL
  end

  config.vm.define "vm4" do |vm4|
    vm4.vm.box = "generic/centos9s"
    vm4.vm.network "private_network", ip: "192.168.56.104"
    vm4.vm.network "public_network", bridge: "enp4s0"

    vm4.vm.provider "virtualbox" do |vb|
      vb.cpus = 2
      vb.memory = "2048"
    end
    vm4.vm.provision "shell", inline: <<-SHELL
      dnf update
    SHELL
  end
end
