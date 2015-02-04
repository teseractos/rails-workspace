Vagrant.configure(2) do |config|
  config.vm.box = "mechfish/precise64-ruby"
  config.vm.network :forwarded_port, host: 3000, guest: 3000
  config.vm.provision "shell", inline: "apt-get install git"
    
  # Proxy config
  # config.proxy.http = ""
  # config.proxy.https = ""
  # config.proxy.no_proxy = "localhost,127.0.0.1"
end