#This is a model to create a swarm and node.
# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|

config.vm.define "docker-swarm" do |swarm|
swarm.vm.box = "centos/7"
swarm.vm.network "private_network", ip: "192.168.33.200"
swarm.vm.hostname = "master"
config.vm.provider "virtualbox" do |v|
	v.memory = 1048
	v.cpus = 2
end

end

config.vm.define "node2" do |node2|
node2.vm.box = "ubuntu/xenial64"
node2.vm.hostname = 'node2'
node2.vm.network :private_network, ip: "192.168.33.201"

end
end
#node1.vm.box = "bento/centos-6.7"
#node1.vm.hostname = 'node1'
#node1.vm.network :private_network, ip: "192.168.33.202"
#end
