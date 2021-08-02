Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/xenial64"
  config.vm.hostname = "appsrv01"
  config.vm.synced_folder "files/", "/home/vagrant/"

  config.vm.network "private_network", ip: "192.168.33.11" # work only on this ip

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 4096
    vb.cpus = 1
  end

  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get -qq update && sudo apt-get -qq upgrade
    add-apt-repository ppa:openjdk-r/ppa -y
    apt-get update
    apt-get -y install apache2 openjdk-8-jdk
    usermod -a -G sudo vagrant
  SHELL

end