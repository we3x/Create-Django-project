# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
    config.vm.box = "debian"
    config.vm.box_url = "https://ftp.lugons.org/vagrant/debian-8.0-x86_64.box"
    config.vm.network :private_network, ip: "192.168.33.10"
    config.vm.provision :ansible do |ansible|
        ansible.playbook = "provision/site.yml"
    end
end
