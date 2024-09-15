Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.network "private_network", type: "dhcp"


  config.vm.network "forwarded_port", guest: 8080, host: 8080


  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end

