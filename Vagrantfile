Vagrant::Config.run do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.forward_port 8124, 8124
  config.vm.provision :shell,
    :inline => "sudo apt-get update && sudo apt-get -y install build-essential git ruby2.1.1 && sudo gem install github-pages therubyracer --no-ri --no-rdoc"

  config.ssh.forward_agent = true
end
