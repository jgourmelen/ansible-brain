# -*- mode: ruby -*-
# vi: set ft=ruby :


VAGRANTFILE_API_VERSION = "2"
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "generic/rhel8"

  #Infra
  config.vm.define "myredhat" do |myredhat|
    myredhat.vm.hostname = "myredhat"
    myredhat.vm.network "private_network", ip: "192.168.10.100"
    myredhat.vm.network "forwarded_port", guest: 443, host: 8443

  end

=begin
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "infra_prerequis.yml"
  end
=end
end
