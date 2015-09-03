# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  # Use the same key for each machine 
  config.ssh.insert_key = false

  config.vm.define "vagrant1" do |vagrant1|
      vagrant1.vm.box = "ubuntu/trusty64"
      vagrant1.vm.network "forwarded_port", guest: 80, host: 8001
      vagrant1.vm.network "forwarded_port", guest: 8080, host: 8080
  end
end
