# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "boxcutter/centos71"
  config.vm.network "private_network", ip: "10.1.1.123"

  config.vm.provision "shell", inline: "sudo yum install -y https://bintray.com/artifact/download/jfrog/artifactory-rpms/artifactory-3.6.0.rpm"
  config.vm.provision "shell", inline: "sudo yum install -y java"
  config.vm.provision "shell", inline: "sudo systemctl start artifactory"
end
