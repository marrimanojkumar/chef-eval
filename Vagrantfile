    
Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-5.11-i386"
  config.vm.network "private_network", type: "dhcp"
  config.vm.boot_timeout = 700
  config.omnibus.chef_version = :latest
  config.vm.provision :chef_client do |chef|
    chef.provisioning_path = "/etc/chef"
    chef.chef_server_url = "https://api.chef.io/organizations/unigo456"
    chef.validation_key_path = ".chef/marrimanoj.pem"
    chef.validation_client_name = "marrimanoj"
    chef.node_name = "centos-server"
  end
end










































