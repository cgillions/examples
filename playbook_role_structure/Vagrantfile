Vagrant.configure(2) do |config|

    # Configure the VM.
    config.vm.box = "centos/7"
    config.vm.hostname = "webserver"
    config.vm.network "private_network", ip: "172.30.20.10"

    # Enable VirtualBox NAT DNS.
    config.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      end
end
