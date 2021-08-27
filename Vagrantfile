# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "bento/ubuntu-20.04"

    config.vm.hostname = "yessbox"

    config.vm.network "forwarded_port", guest: 80, host: 8080
    config.vm.network "private_network", ip: "192.168.33.10"

    config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]

end
