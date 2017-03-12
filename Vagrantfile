# -*- mode: ruby -*-
# vi: set ft=ruby :


Vagrant.configure("2") do |config|

  config.vm.box = "bento/centos-7.3"



  config.vm.provision "shell", inline: <<-SHELL
    yum install -y epel-release
    yum install -y python-pip
    yum install -y python-devel
    yum group install -y "Development Tools"
    yum install -y openssl-devel
    pip install --upgrade pip
    pip install virtualenv
    pip install ansible
    pip install setuptools -U

  SHELL
end
