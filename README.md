# centos8-remote-dir
Instruction for instaling remote dir on centos8 with Vbox

yum update kernel*

reboot

mkdir /media/VBoxLinuxAdditions

mount -r /dev/cdrom /media/VBoxLinuxAdditions

yum install epel-release

yum install kernel-devel kernel-headers gcc make dkms perl bzip2

KERN_DIR=/usr/src/kernels/uname -r

export KERN_DIR

cd /media/VBoxLinuxAdditions

./VBoxLinuxAdditions.run
