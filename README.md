# CMPE283 : Virtualization </br>
Assignment 2: Modifying instruction behavior in KVM </br>
Group:</br>
Yifan Liu (011410984)</br>
Binwang Luo(014632566) </br>

Respons：</br>
Yifan Liu:</br>
a. Builing the Kernel to last version </br>
b. got Nested VM  </br> 
c. Modify the CPUID emulation code in KVM to report back additional information </br>
d. Testing assignment </br>
e. Verify proper output </br>

Binwang Luo(014632566)</br>
a. Wrote the test program </br>
b. Detemine where to place the measurement code </br>
c. Create new CPID leaf 0x4fffffff </br>
d. Updated documents to github</br>

Steps as below:  

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
e. apt-get install virt-manager</br>
f. virsh version </br>
</br>

4. install subline text  </br>
a. sudo apt install gcc  </br>
b. sudo apt install apt-transport-https ca-certificates curl software-properties-common  </br>
c. curl -fsSL https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -  </br>
d. sudo add-apt-repository "deb https://download.sublimetext.com/ apt/stable/"  </br>
d. sudo apt install sublime-text  </br>
 </br>
5.Edit the file cpuil.c and vmx.c  </br>
 </br>

Question 3:  </br>
a. Does the number of exits increase at a stable rate?Or are there
more exits performed during certain VM operations? </br>
After the CPUID function executing, the number of exits increasing.  
b. How many exits does a full VM boot entail? </br>
There are approximately 24 millions exits. 


