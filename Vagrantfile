Vagrant.configure(2) do |config|
  config.vm.define "node1" do |node1| 
    node1.vm.box = "ubuntu/trusty64"
    node1.vm.network "public_network" , :adapter=>2 , type: "dhcp", :bridge => "Realtek PCIe GBE Family Controller"
    node1.vm.hostname ="node1"
    node1.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
    vb.gui = true
    vb.name = "node1"
     # Customize the amount of memory on the VM:
    vb.memory = "512"
    end 
end
config.vm.define "node2" do |node2| 
    node2.vm.box = "centos/7"
    node2.vm.network "public_network" , :adapter=>2 , type: "dhcp", :bridge => "Realtek PCIe GBE Family Controller"
    node2.vm.hostname ="node2"
    node2.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
    vb.gui = true
    vb.name = "node2"
     # Customize the amount of memory on the VM:
    vb.memory = "512"
    end 
end
end