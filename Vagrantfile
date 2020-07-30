# -*- mode: ruby -*-
# vi: set ft=ruby :

ENV['VAGRANT_NO_PARALLEL'] = 'yes'

Vagrant.configure(2) do |config|


  # Kubernetes Master Server
  config.vm.define "dep" do |ktmaster|
    ktmaster.vm.box = "centos/7"
    ktmaster.vm.hostname = "dep.example.com"
    ktmaster.vm.network "public_network", ip: "192.168.224.230", bridge: "vmnet8"
    ktmaster.vm.provider "virtualbox" do |v|
      v.name = "dep"
      v.memory = 1024
      v.cpus = 1
    end
  end

end
