# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  # come from https://github.com/tknerr/vagrant-docker-baseimages
  config.vm.provider "docker" do |d|
    d.image = "tknerr/baseimage-ubuntu:22.04"
    d.has_ssh = true
  end

  config.vm.provision "shell", inline: <<-SHELL
    apt-get update -y
  SHELL
end
