# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  
      NODENUM = 2

      (1..NODENUM).each do |i|
            config.vm.define "node-#{i}" do |node|

                  node.vm.box = "centos7.4"

                  node.vm.hostname = "node-#{i}"

                  node.vm.post_up_message = "node-#{i} init success"

                  # node.ssh.username = "vagrant"

                  # node.ssh.password = "vagrant"

                  #node.ssh.port = "2222"

                  node.ssh.keep_alive = "60" 

                  # config.vm.network "forwarded_port", guest: 80, host: 8080

                  # config.vm.network "forwarded_port", guest: 80, host: 8080, host_ip: "127.0.0.1"

                  # config.vm.network "private_network", ip: "192.168.33.10"

                  # config.vm.network "public_network"

                  # config.vm.synced_folder "../data", "/vagrant_data"
            
                  node.vm.provider "virtualbox" do |vb|

                        #   vb.gui = true

                        vb.name = "node-#{i}"

                        vb.memory = "1024"

                        vb.cpus = "1"
                  end
            
            
                  # config.vm.provision "shell", inline: <<-SHELL
                  #   apt-get update
                  #   apt-get install -y apache2
                  # SHELL
            
            end
      end      
end
