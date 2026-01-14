# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
  # Ortak ayarlar
  config.vm.box = "ubuntu/bionic64"
  config.ssh.insert_key = false

  # 1. MAKİNE: Control Node
  config.vm.define "control_node" do |control|
    control.vm.hostname = "control-node"
    control.vm.network "private_network", ip: "192.168.56.10"
    control.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.name = "Ansible-Control-Node"
    end
  end

  # 2. MAKİNE: Managed Node
  config.vm.define "managed_node" do |node|
    node.vm.hostname = "managed-node"
    node.vm.network "private_network", ip: "192.168.56.20"
    node.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.name = "Ansible-Target-Node"
    end
  end
end