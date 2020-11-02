# CMPE283 : Virtualization </br>
Assignment 2: Modifying instruction behavior in KVM </br>
1. Download the source code: </br>
git clone https://github.com/torvalds/linux.git   </br>
</br>
2. Building The Kernel   </br>
 a. sudo bash   </br>
 b. apt-get install build-essential kernel-package fakeroot libncurses5-dev libssl-dev ccache bison flex libelf-dev  </br>
c. uname -a </br>
d. cp /boot/config-4.15.0-112-generic    ./.config  </br>
e. make oldconfig  </br>
f. make && make modules && make install && make modules_install  </br>
g. reboot  </br>
h. uname -r  </br>
</br>

3. install VM manager
a. sudo bash   </br>
b. apt install cpu-checker  </br>
c. kvm-ok  </br>
d. apt-get install qemu-kvm libvirt-daemon-system libvirt-clients bridge-utils    </br>
e. virsh version </br>
</br>

4. 
