Vagrant.configure(2) do |config|

  config.vm.box = "geerlingguy/centos6"

  config.vm.box_check_update = false

  config.vm.hostname = "fadi-centos6"
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "2048"
  end

  config.vm.provision :ansible do |ansible|
            # ansible.verbose='vvvv'
            ansible.sudo = true
            ansible.limit = 'all'
            ansible.playbook = 'fadi.yml'
    end

end
