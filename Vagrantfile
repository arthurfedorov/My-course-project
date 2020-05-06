Vagrant.configure("2") do |config|

  config.vm.define "web1" do |box|
    box.vm.box = "centos/8"
    box.vm.hostname = "web1.homelab.loc"
    
    box.vm.network :private_network, ip: "192.168.10.100"

    box.vm.box_check_update = false

    box.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "2048","--cpus", "2"]
    end
  end

  config.vm.define "web2" do |box|
    box.vm.box = "centos/8"
    box.vm.hostname = "web2.homelab.loc"
    
    box.vm.network :private_network, ip: "192.168.10.101"

    box.vm.box_check_update = false

    box.vm.provider :virtualbox do |vb|
      vb.customize ["modifyvm", :id, "--memory", "2048","--cpus", "2"]
    end
  end

  config.vm.define "web3" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "web3.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.102"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "2048","--cpus", "2"]
      end
  end

  config.vm.define "pg1" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "pg1.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.110"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "4096","--cpus", "4"]
      end
  end

  config.vm.define "pg2" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "pg2.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.111"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "4096","--cpus", "4"]
      end
  end

  config.vm.define "pg3" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "pg3.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.112"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "4096","--cpus", "4"]
      end
  end

  config.vm.define "haproxy1" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "haproxy1.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.120"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "2"]
      end
  end

  config.vm.define "haproxy2" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "haproxy2.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.121"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "2"]
      end
  end

  config.vm.define "haproxy3" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "haproxy3.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.122"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "2"]
      end
  end

  config.vm.define "rabbitmq1" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "rabbitmq1.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.130"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "2"]
      end
  end

  config.vm.define "rabbitmq2" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "rabbitmq2.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.131"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "2"]
      end
  end

  config.vm.define "rabbitmq3" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "rabbitmq3.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.132"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "1024","--cpus", "2"]
      end
  end

  config.vm.define "consul" do |box|
      box.vm.box = "centos/8"
      box.vm.hostname = "consul.homelab.loc"
      
      box.vm.network :private_network, ip: "192.168.10.140"
  
      box.vm.box_check_update = false
  
      box.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "2048","--cpus", "4"]
      end
  end

  # config.vm.define "prometheus" do |box|
  #     box.vm.box = "centos/8"
  #     box.vm.hostname = "prometheus.homelab.loc"
      
  #     box.vm.network :private_network, ip: "192.168.10.170"
  
  #     box.vm.box_check_update = false
  
  #     box.vm.provider :virtualbox do |vb|
  #       vb.customize ["modifyvm", :id, "--memory", "4096","--cpus", "4"]
  #     end
  # end

  # config.vm.define "grafana" do |box|
  #     box.vm.box = "centos/8"
  #     box.vm.hostname = "grafana.homelab.loc"
      
  #     box.vm.network :private_network, ip: "192.168.10.171"
  
  #     box.vm.box_check_update = false
  
  #     box.vm.provider :virtualbox do |vb|
  #       vb.customize ["modifyvm", :id, "--memory", "2048","--cpus", "2"]
  #     end
  # end

end