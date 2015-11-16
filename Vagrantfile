Vagrant::Config.run do |config|

  config.vm.box = "ubuntu/trusty64"
  config.vm.forward_port 8124, 8124
  config.vm.provision :shell,
    :inline => "sudo apt-add-repository ppa:rael-gc/rvm && sudo apt-get update && sudo apt-get install -y git-core curl zlib1g-dev build-essential libssl-dev libreadline-dev libyaml-dev libsqlite3-dev sqlite3 libxml2-dev libxslt1-dev libcurl4-openssl-dev python-software-properties libffi-dev rvm && rvm install 2.1.1 && rvm use 2.1.1 --default && echo 'gem: --no-ri --no-rdoc' > ~/.gemrc && sudo gem install bundler jekyll github-pages --no-rdoc --no-ri"

  config.ssh.forward_agent = true
end
