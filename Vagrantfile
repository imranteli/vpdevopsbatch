Vagrant.configure("2") do |config|

### Webserver
### Centos virtual machine with bridge interface and 512 mb memory 
  config.vm.define "web" do |web|
    web.vm.box = "nrel/CentOS-6.5-x86_64"
    web.vm.hostname = 'web'
    web.vm.network "public_network", bridge: "wlo1"
    web.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--memory", 512]
    end
  end

### DBserver
### Centos virtual machine with bridge interface and 512 mb memory 
  config.vm.define "db" do |db|
    db.vm.box = "nrel/CentOS-6.5-x86_64"
    db.vm.hostname = 'db'
    db.vm.network "public_network", bridge: "wlo1"
    db.vm.provider :virtualbox do |v|
      v.customize ["modifyvm", :id, "--memory", 512]
    end

  end
end
