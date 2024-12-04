Vagrant.configure("2") do |config|
    config.vm.box = "bento/ubuntu-22.04"
    config.vm.hostname = 'jenkins'
    config.vm.network 'forwarded_port', guest: 8080, host: 8080, host_ip: '127.0.0.1'
    config.vm.provision 'shell', path: 'provision.sh'
    config.vm.provider 'virtualbox' do |v|
        v.memory = 2048
    end
end