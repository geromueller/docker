$script = <<SCRIPT

sudo tee /etc/apt/sources.list <<EOF
deb http://httpredir.debian.org/debian jessie main
deb http://httpredir.debian.org/debian jessie-backports main
deb http://security.debian.org/ jessie/updates main
EOF

# ----------------------------------------------------------------------
# install packages
# ----------------------------------------------------------------------
sudo apt update
sudo apt --assume-yes install -t jessie-backports -y docker.io

SCRIPT
  
  
Vagrant.configure(2) do |config|
  config.vm.box = "debian/contrib-jessie64"

  config.vm.provision "shell", inline: $script
end
