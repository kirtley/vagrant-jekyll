Vagrant::Config.run do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.forward_port 8124, 8124
  config.vm.provision :shell,
    :inline => "sudo apt-get update && sudo apt-get install -y ruby ruby-dev make gcc nodejs git-core && sudo gem install jekyll github-pages --no-rdoc --no-ri"

  config.ssh.forward_agent = true
end
