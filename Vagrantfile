$up_script = <<ALWAYSRUN
pwd
ALWAYSRUN

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.hostname = "my-project"
  config.vm.network "private_network", ip: "192.168.52.52"

  config.vm.synced_folder ".", "/vagrant"

  config.vm.provision "shell", path: "provision.sh"
end
