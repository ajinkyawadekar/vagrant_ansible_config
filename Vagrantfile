Vagrant.configure("2") do |config|
#  config.vm.network "forwarded_port", guest: 22, host: 2222
    config.vm.box = "centos/7"
    config.vm.define "server"
    config.vm.define "client"
  config.vm.provision :ansible do |ansible|
    ansible.verbose = "vv"
    ansible.playbook = "provision/ldap_server.yml"
  end
end

