Vagrant.configure("2") do |config|
    config.vm.box = "bento/ubuntu-22.04"
    config.vm.hostname = 'jenkins'
    config.vm.network 'forwarded_port', guest: 8080, host: 8080, host_ip: '127.0.0.1'
    config.vm.network 'forwarded_port', guest: 8091, host: 8091, host_ip: '127.0.0.1'
    config.vm.network "private_network", ip: "192.168.56.7"
    config.vm.provision 'shell', path: 'provision-latest.sh'
    config.vm.provider 'virtualbox' do |v|
        v.memory = 4096
    end
end