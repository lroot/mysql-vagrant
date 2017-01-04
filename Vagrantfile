# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
    config.vm.box = "trusty64"
    config.vm.box_url = "https://cloud-images.ubuntu.com/vagrant/trusty/current/trusty-server-cloudimg-amd64-vagrant-disk1.box"
    config.vm.box_download_checksum = "e2890d8862fb7ab5092563a97644a17da4ba42084d7e919ddd9f14cc78fe3993"
    config.vm.box_download_checksum_type = "sha256"

    config.vm.host_name = "mysql-server.local" # OPTIONAL - Update to your hosts file will be needed to map this
    config.vm.network :private_network, ip: "192.168.1.44"
    config.vm.provision :shell, :path => "install.sh"
end
