# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-18.04"
  config.vm.provider :hyperv do |hyperv|
    hyperv.vmname = "TestVM"
    hyperv.cpus = 2
    hyperv.maxmemory = 4000
  end
  config.vm.network "public_network", bridge: "lan"
  config.vm.synced_folder '.', '/vagrant', disabled: true
end
