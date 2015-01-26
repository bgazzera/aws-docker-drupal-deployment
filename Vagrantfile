Vagrant.configure("2") do |config|

  config.vm.define "app" do |app|
    app.vm.provider "docker" do |d|
      d.build_dir = "./"
      d.vagrant_vagrantfile = "VagrantfileDockerHost"
      d.remains_running = true
      d.ports = ["8080:80"]
    end
  end
end