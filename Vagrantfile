Vagrant.configure("2") do |config|
  config.vm.box = "peru/ubuntu-18.04-desktop-amd64"
  config.vm.box_version = "20180801.01"
  config.vm.provision "file", source: "~/Projects/ansible-ubuntu", destination: "/tmp/ansible-ubuntu"
  config.vm.provision "shell",
    inline: "/bin/sh /tmp/ansible-ubuntu/install.sh"
end
