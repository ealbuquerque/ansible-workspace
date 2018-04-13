Vagrant.configure("2") do |config|

  config.vm.synced_folder ".", "/vagrant_data"
  
  config.ssh.insert_key = false

  config.vm.define "vagrantdev" do |vagrantdev|
    vagrantdev.vm.box = "ubuntu/artful64"
  end

end
