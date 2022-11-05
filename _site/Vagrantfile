# -*- mode: ruby -*-
# vi: set ft=ruby :
 
Vagrant.configure("2") do |config|

  config.vm.box = "hashicorp/bionic64"
  
  config.vm.network "forwarded_port", guest: 4000, host: 4000
 
 
  # config.vm.provider "virtualbox" do |vb|
  #   # Display the VirtualBox GUI when booting the machine
  #   vb.gui = false
   
  #   vb.memory = "1024"
  # end
 
  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    sudo apt-get install -y build-essential nodejs ruby-full zlib1g-dev
    echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
    echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
    echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
    source ~/.bashrc
    sudo gem update --system
    sudo gem install github-pages
    sudo gem install jekyll bundler
  SHELL
end
