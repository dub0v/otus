
Vagrant.configure("2") do |config|
  config.vm.box = "centos/8"
  config.vm.box_check_update = true
  config.vm.hostname = "core"  
  config.vm.network "public_network", ip: "192.168.1.100"
  config.vm.define "coreup"
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
    end

end
