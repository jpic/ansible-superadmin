# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.define "arch" do |arch|
    arch.vm.box = "terrywang/archlinux"

    arch.vm.provision "ansible" do |ansible|
        ansible.playbook = "test.yml"
        ansible.extra_vars = {
            ansible_python_interpreter: "/usr/bin/python2",
            ansible_ssh_user: 'vagrant',
            user: 'james',
        }
    end
  end
end
