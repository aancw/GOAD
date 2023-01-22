#########################################
#  ESXI Provider host/login details
#########################################
#
#   Use of variables here to hide/move the variables to a separate file
#
provider "esxi" {
  esxi_hostname = var.esxi_hostname
  esxi_hostport = var.esxi_hostport
  esxi_username = var.esxi_username
  esxi_password = var.esxi_password
}

#########################################
#  ESXI Guest resource
#########################################

resource "esxi_guest" "DC01" {
  guest_name = "DC01"
  disk_store = var.esxi_datastore
  guestos    = "windows9srv-64"

  boot_disk_type = "thin"

  memsize            = "4000"
  numvcpus           = "2"
  resource_pool_name = "/"
  power              = "on"
  clone_from_vm = "WindowsServer2019"
  # This is the network that bridges your host machine with the ESXi VM
  network_interfaces {
    virtual_network = var.vm_network
  }
  guest_startup_timeout  = 45
  guest_shutdown_timeout = 30
}

resource "esxi_guest" "DC02" {
  guest_name = "DC02"
  disk_store = var.esxi_datastore
  guestos    = "windows9srv-64"

  boot_disk_type = "thin"

  memsize            = "4000"
  numvcpus           = "2"
  resource_pool_name = "/"
  power              = "on"
  clone_from_vm = "WindowsServer2019"
  # This is the network that bridges your host machine with the ESXi VM
  network_interfaces {
    virtual_network = var.vm_network
  }
  guest_startup_timeout  = 45
  guest_shutdown_timeout = 30
}

resource "esxi_guest" "DC03" {
  guest_name = "DC03"
  disk_store = var.esxi_datastore
  guestos    = "windows9srv-64"

  boot_disk_type = "thin"

  memsize            = "4000"
  numvcpus           = "2"
  resource_pool_name = "/"
  power              = "on"
  clone_from_vm = "WindowsServer2016"
  # This is the network that bridges your host machine with the ESXi VM
  network_interfaces {
    virtual_network = var.vm_network
  }
  guest_startup_timeout  = 45
  guest_shutdown_timeout = 30
}

resource "esxi_guest" "SRV02" {
  guest_name = "SRV02"
  disk_store = var.esxi_datastore
  guestos    = "windows9srv-64"

  boot_disk_type = "thin"

  memsize            = "4000"
  numvcpus           = "2"
  resource_pool_name = "/"
  power              = "on"
  clone_from_vm = "WindowsServer2019"
  # This is the network that bridges your host machine with the ESXi VM
  network_interfaces {
    virtual_network = var.vm_network
  }
  guest_startup_timeout  = 45
  guest_shutdown_timeout = 30
}
resource "esxi_guest" "SRV03" {
  guest_name = "SRV03"
  disk_store = var.esxi_datastore
  guestos    = "windows9srv-64"

  boot_disk_type = "thin"

  memsize            = "4000"
  numvcpus           = "2"
  resource_pool_name = "/"
  power              = "on"
  clone_from_vm = "WindowsServer2016"
  # This is the network that bridges your host machine with the ESXi VM
  network_interfaces {
    virtual_network = var.vm_network
  }
  guest_startup_timeout  = 45
  guest_shutdown_timeout = 30
}