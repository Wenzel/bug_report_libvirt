Vagrant.configure(2) do |config|
    config.vm.box = "debian/jessie64"

    config.vm.synced_folder ".", "/vagrant", disabled: true

    config.vm.provision "ansible" do |ansible|
        ansible.playbook = "playbook.yml"
    end
end
