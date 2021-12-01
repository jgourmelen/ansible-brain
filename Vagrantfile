# -*- mode: ruby -*-
# vi: set ft=ruby :


VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "generic/rhel8"

  #Infra
  config.vm.define "myredhat" do |master|
    master.vm.hostname = "myredhat"
    master.vm.network "private_network", ip: "192.168.10.100"
  end

=begin
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "infra_prerequis.yml"
  end
=end
end
