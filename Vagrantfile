# -*- mode: ruby -*-
# vim: set ft=ruby :

MACHINES = {
  :web => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.100'
  },
  :pg => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.110'
  },
  :redis => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.120'
  },
  :rabbitmq => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.130'
  }
}

Vagrant.configure("2") do |config|

  MACHINES.each do |boxname, boxconfig|

      config.vm.define boxname do |box|

          box.vm.box = boxconfig[:box_name]
          box.vm.host_name = boxname.to_s

          box.vm.network "private_network", ip: boxconfig[:ip_addr]

          box.vm.provider :virtualbox do |vb|
          
          case boxname.to_s
          when "web"
            vb.customize ["modifyvm", :id, "--memory", "1024"]
          when "pg"
            vb.customize ["modifyvm", :id, "--memory", "512"]
          end

          end

      end
  end
end
