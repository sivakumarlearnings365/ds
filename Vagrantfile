Vagrant.configure("2") do |config|
  config.hostmanager.enabled = true
  config.hostmanager.manage_host = true

## 01 VM ##
config.vm.define "box1" do |box1|
    box1.vm.box = "centos/stream9"
    box1.vm.hostname = "box1"
    box1.vm.network "private_network", ip: "192.168.56.20"
    box1.vm.provider "virtualbox" do |vb|
     vb.memory = "2048"
   end

  end
end
  



