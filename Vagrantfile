Vagrant.configure("2") do |config|

  config.vm.box = "geerlingguy/ubuntu1604"

  config.vm.provider "virtualbox" do |v|
    v.name = "ansible_do_env"
  end

  config.vm.provision "shell", inline: <<-SHELL
    apt-add-repository ppa:ansible/ansible
    apt-get update
    apt-get install -y ansible python-pip
    export LC_ALL=C 
    pip install --upgrade pip
    pip install dopy
  SHELL
end