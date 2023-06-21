IMAGE_NAME = "ubuntu/jammy64"
N = 3

Vagrant.configure("2") do |config|
    config.ssh.insert_key = false

    config.vm.provider "virtualbox" do |v|
        v.memory = 2048
        v.cpus = 2
    end

    (1..N).each do |i|
        config.vm.define "microk8s-node-#{i}" do |node|
            node.vm.provider :virtualbox do |vm|
                vm.name = "microk8s-node-#{i}"
            end
            node.vm.box = IMAGE_NAME
            node.vm.network "private_network", ip: "192.168.56.#{i + 50}"
            node.vm.hostname = "microk8s-node-#{i}"    
            # node.vm.provision "ansible" do |ansible|
                # ansible.verbose = "v"
                # ansible.playbook = "playbooks/additional-packages-playbook.yml"
            # end
        end
    end
end
