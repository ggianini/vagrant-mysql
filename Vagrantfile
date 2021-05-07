Vagrant.configure("2") do |config|
  config.vm.box = "centos/7"
  config.vm.hostname = "Infra-e-Cloud-01"
  config.vm.network "private_network", ip: "192.168.100.20"
  config.vm.network :forwarded_port, guest: 3306, host: 3306
  config.vm.provision :shell, path: "bootstrap.sh"
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "1024"
    vb.cpus = "2"
    end
   end