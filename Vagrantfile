Vagrant.configure("2") do |config|
  ############
  # First VM #
  ############
  config.vm.define "main" do |main|
    main.vm.box = "centos/7"
    main.vm.box_check_update = false
    main.vm.hostname = 'main'

    main.vm.network :private_network, ip: "192.168.56.101"

    main.vm.provider :virtualbox do |v|
      v.name = "main"
    end

    main.vm.synced_folder "/devdir", "/vagrant_data"
  end

  #############
  # Second VM #
  #############
  config.vm.define "second" do |second|
    second.vm.box = "centos/7"
    second.vm.box_check_update = false
    second.vm.hostname = 'second'

    second.vm.network :private_network, ip: "192.168.56.102"

    second.vm.provider :virtualbox do |v|
      v.name = "second"
    end

    second.vm.synced_folder "/devdir", "/vagrant_data"
  end

end
