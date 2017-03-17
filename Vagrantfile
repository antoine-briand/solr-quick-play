Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible-playbook.yml"
  end
  config.vm.network "forwarded_port", guest: 8983, host: 8983
end
