Vagrant.configure("2") do |config|
  config.hostmanager.enabled = true
  config.hostmanager.manage_host = true

## 01 VM ##
config.vm.define "centos01" do |centos01|
    centos01.vm.box = "centos/stream9"
    centos01.vm.hostname = "centos01"
    centos01.vm.network "private_network", ip: "192.168.56.20"
    centos01.disksize.size = '60GB'
    centos01.vm.provider "virtualbox" do |vb|
     vb.memory = "4548"
     
   end

  end

    ## 02 VM ##
config.vm.define "centos02" do |centos02|
    centos02.vm.box = "centos/stream9"
    centos02.vm.hostname = "centos02"
    centos02.vm.network "private_network", ip: "192.168.56.21"
    centos02.disksize.size = '60GB'
    centos02.vm.provider "virtualbox" do |vb|
     vb.memory = "2048"
   end

  end

    ## 03 VM ##
  config.vm.define "ubuntu01" do |ubuntu01|
    ubuntu01.vm.box = "bento/ubuntu-24.04"
    ubuntu01.vm.hostname = "ubuntu01"
    ubuntu01.vm.network "private_network", ip: "192.168.56.23"
    ubuntu01.disksize.size = '50GB'
    ubuntu01.vm.provider "virtualbox" do |vb|
       vb.memory = "3548"
     end
  
    end



end
