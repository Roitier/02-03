Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.box_version = "20220113.0.0"

  config.vm.provider "libvirt" do |libvirt|
    libvirt.cpus = 2
    libvirt.memory = "1024"
  end

  config.vm.synced_folder ".", "/ramildo_junior"

  config.vm.network :private_network, ip: "192.168.1.254"

  config.vm.network :forwarded_port, guest: 80, host: 80, host_ip: "127.0.0.1", auto_correct: true

end



