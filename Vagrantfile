Vagrant.configure("2") do |config|
    config.vm.box = "centos/7"
    config.vm.define "server"
  config.vm.provision :ansible do |ansible|
#    ansible.verbose = "v"
    ansible.playbook = "provision/ldap_server.yml"
  end
end
Vagrant.configure("2") do |config|
    config.vm.define "client"
  config.vm.provision :ansible do |ansible|
#    ansible.verbose = "v"
    ansible.playbook = "provision/ldap_client.yml"
  end
end
