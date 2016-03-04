# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "boxcutter/ubuntu1404"
  config.vm.define "ubuntu-vault" do |cfg| 
    cfg.vm.hostname="ubuntu-vault"
    cfg.vm.box_check_update = true

    cfg.vm.provider :virtualbox do |vbox, override|
      vbox.customize ["modifyvm", :id,
                      "--name", "ubuntu-vault",
                      "--memory", 1024,
                      "--cpus", 1
      ]
    end
  end
end
