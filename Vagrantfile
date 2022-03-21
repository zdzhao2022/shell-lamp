# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.box = "geerlingguy/centos7"
  
  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.provision "file",
    source: "~/vagrant/file/git-config",
	destination: "~/.gitconfig"
	
  config.vm.provision "shell", 
    path: "https://raw.githubusercontent.com/zdzhao2022/vagrant/main/scripts/centos-lamp.sh"
  
end
