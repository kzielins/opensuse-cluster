# -*- mode: ruby -*-
# vi: set ft=ruby :

BOX_IMAGE = "bento/opensuse-leap-42.1"
NODE_COUNT = 2

Vagrant.configure("2") do |config|
  (1..NODE_COUNT).each do |i|
    config.vm.define "node#{i}" do |subconfig|
      subconfig.vm.box = BOX_IMAGE
                subconfig.vm.hostname = "node#{i}"
      subconfig.vm.network :private_network, ip: "10.0.30.#{i + 10}"
    end
  end



end 

