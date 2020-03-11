# -*- mode: ruby -*-
# vi: set ft=ruby :

vmname = "vm-ansible"

Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.hostname = vmname
  config.ssh.keep_alive = true
  config.vm.box_check_update = true
  config.vm.network "public_network", use_dhcp_assigned_default_route: true
  config.vm.synced_folder "./vagrant_data", "/vagrant_data"
  config.vm.provider "virtualbox" do |vb|
    vb.gui = false
    vb.memory = "1024"
    vb.name = vmname
   end  
end
