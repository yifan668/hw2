# CMPE283 : Virtualization </br>
Assignment 2: Modifying instruction behavior in KVM </br>
Group:</br>
Yifan Liu (011410984)</br>
respons：</br>
1. got the Kernel to last version </br>
2. got Nested VM  </br>
3. Wrote the test program </br>
4. Modify the CPUID emulation code in KVM to report back additional information </br>
5. Moddify the kernel code with the assignment functionality </br>
a. Detemine where to place the measurement code </br>
b. Create new CPID leaf 0x4fffffff </br>
6.Testing assignment </br>
7. Verify proper output </br>

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

3. install VM manager  </br>
a. sudo bash   </br>
b. apt install cpu-checker  </br>
c. kvm-ok  </br>
d. apt-get install qemu-kvm libvirt-daemon-system libvirt-clients bridge-utils    </br>
e. </br>
f. virsh version </br>
</br>

4. install subline text  </br>
a. sudo apt install gcc  </br>
b. sudo apt install apt-transport-https ca-certificates curl software-properties-common  </br>
c. curl -fsSL https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -  </br>
d. sudo add-apt-repository "deb https://download.sublimetext.com/ apt/stable/"  </br>
d. sudo apt install sublime-text  </br>
 </br>
