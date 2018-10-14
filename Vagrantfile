Vagrant.configure("2") do |config|

  config.vm.box = "centos/7"
  config.vm.box_check_update = false

  config.vm.provider "virtualbox" do |vm|
    vm.name = "dev"
  end

  config.vm.synced_folder "/Users/hazriqishak/Documents/dev", "/vagrant_data"
  
end
