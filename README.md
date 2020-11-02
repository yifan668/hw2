# CMPE283 : Virtualization </br>
Assignment 2: Modifying instruction behavior in KVM </br>
1. Download the source code: </br>
&nbsp  git clone https://github.com/torvalds/linux.git   </br>
</br>
2.Building The Kernel   </br>
&nbsp a. sudo bash   </br>
&nbsp b. apt-get install build-essential kernel-package fakeroot libncurses5-dev libssl-dev ccache bison flex libelf-dev  </br>
&nbsp c. uname -a </br>
&nbsp d. cp /boot/config-4.15.0-112-generic    ./.config  </br>
&nbsp e. make oldconfig  </br>
&nbsp f. make && make modules && make install && make modules_install  </br>
&nbsp g.reboot  </br>
&nbsp uname -r  </br>
</br>
