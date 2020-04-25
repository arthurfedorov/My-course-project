# -*- mode: ruby -*-
# vim: set ft=ruby :

MACHINES = {
  :web1 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.100'
  },

  :web2 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.101'
  },

  :web3 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.102'
  },

  :pg1 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.110'
  },
   
  :pg2 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.111'
  },

  :pg3 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.112'
  },

  :haproxy1 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.120'
  },

  :haproxy2 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.121'
  },

  :haproxy3 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.122'
  },

  :rabbitmq1 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.130'
  },

  :rabbitmq2 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.131'
  },

  :rabbitmq3 => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.132'
  },

  :redis => {
        :box_name => "centos/8",
        :ip_addr => '192.168.10.140'
  },
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
