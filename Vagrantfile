# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Указываем базовый образ для виртуальных машин
  config.vm.box = 'becoll/amazonlinux2023'
  config.vm.box_version = '1.0'

  # Первая виртуальная машина
  config.vm.define "vm1" do |vm1|
    vm1.vm.network "private_network", ip: "192.168.33.11"
    vm1.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = "2"
    end
    vm1.vm.provision "shell", inline: <<-SHELL
      sudo yum update -y
    SHELL
  end

  # Вторая виртуальная машина
  config.vm.define "vm2" do |vm2|
    vm2.vm.network "private_network", ip: "192.168.33.12"
    vm2.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = "2"
    end
    vm2.vm.provision "shell", inline: <<-SHELL
      sudo yum update -y
    SHELL
  end

  # Третья виртуальная машина
  config.vm.define "vm3" do |vm3|
    vm3.vm.network "private_network", ip: "192.168.33.13"
    vm3.vm.provider "virtualbox" do |vb|
      vb.memory = "2048"
      vb.cpus = "2"
    end
    vm3.vm.provision "shell", inline: <<-SHELL
      sudo yum update -y
    SHELL
  end
end
