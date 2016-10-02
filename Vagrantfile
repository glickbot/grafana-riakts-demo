# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.network "forwarded_port", guest: 3000, host: 3000
  config.vm.network "forwarded_port", guest: 9000, host: 9000
  config.vm.network "forwarded_port", guest: 8086, host: 8086
  config.vm.network "forwarded_port", guest: 8087, host: 8087
  config.vm.network "forwarded_port", guest: 8098, host: 8098

  config.vm.box = "ubuntu/trusty64"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = "4096"
  end
  config.vm.hostname = "riakts.local"

  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
