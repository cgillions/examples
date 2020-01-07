Vagrant.configure(2) do |config|

    # Configure the VM.
    config.vm.box = "centos/7"
    config.vm.hostname = "webserver"
    config.vm.network "private_network", ip: "172.30.20.10"

    # Enable VirtualBox NAT DNS.
    # Not usually required, but I had an issue with the VM not resolving DNS names.
    config.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
      end
end
