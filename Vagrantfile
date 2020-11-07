# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  # Every Vagrant development environment requires a box. You can search for
  # boxes at https://vagrantcloud.com/search.
  config.vm.box = "archLinux/archLinux"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbooks/dev-env.yaml"
  end
end
