* setup linux
* install qemu
* build windows disk image file
* download windows iso
* download virtio driver iso
* start up qemu with windows
* vnc to qemu instance
* install windows
* copy virtio drivers into image
* enable rdp
* sysprep to audit mode > shutdown
* gzip image
* move image to do using recovery mode
* wget > gunzip > dd of=/dev/vda
* setup digitalocean firewall 
* use recovery console to install drivers
* disable windows firewall, rely on digitalocean firewall only open to your ip
* install drivers
* set network ip manually
* reboot to oobe, no generalize
* set password, then mstsc
* extend partition with diskpart (easy way - remove recovery partition)
* select disk 0, select partition 3, delete partition override
* diskmgmt.msc to extend windows partition
