<center>
#Sri Lanka Institute of Information Technology#
</center>

<br>

</br>

<center>
##Enterprise Standards and Best Practices for IT Infrastructure##
</center>
<br>

</br>
<center>
###4th Year 2nd Semester 2016###
###Bare-metal Installation Summary Report###
</center>

----------

####Name :  Perera K. A. U####
####SLIIT ID :  IT13019600####
####Practical Session: WD (Friday 3.30 pm- 5.30 pm)####

####GITHUB URL:####




----------
----------
####Practical Number: Lab 04####
####Practical Title: Bare-metal Installation####
----------
----------


#####Introduction to Bare-metal installation#####

**Hypervisor** is a software that allows multiple operating systems(OSs) to run concurrently on a physical machine and to interact directly with the physical hardware. There are two types of hypervisors. They are,

<pre>* Hosted Hypervisor

* Bare-metal Hypervisor </pre>

Bare-metal hypervisor is an operating system.But the Hosted hypervisor installs and runs like as an application. 

Throughout this report it explains the steps that are followed to do Bare-metal installation.


**Step 01** – First create a new virtual machine.
<pre>File -> New Virtual Machine </pre>

![](http://i.imgur.com/8XExzDr.png)

* Select "Typical" as the configuration type. 

![](http://i.imgur.com/aNETayN.png)

**Step 02** - Browse the ISO image.

 ![](http://i.imgur.com/5Y8bhPW.png)

**Step 03** - Browse the path to file that consists ISO.

![](http://i.imgur.com/uy1SNIr.png)

**Step 04** - Then give a proper name and location for new virtual machine .

![](http://i.imgur.com/O3Z3kvR.png)

**Step 05** - Keep the maximum disk size as 40.0GB as given in New Virtual Machine Wizard. Then select "Store virtual disk as a single file" at the same window.

![](http://i.imgur.com/vxKTx6J.png)

* It's highly recommended to allocate at least 4GB of RAM space. The physical machine you use, need to have more than 4 GB of RAM space to do this. 

<pre> Customize -> Add -> Select RAM size as 4GB </pre>

* Make sure to choose NAT as network adapter.
* Click on "Close" button. 

![](http://i.imgur.com/U86TF7N.png)

**Step 06** - Then click on "Finish button" New Virtual Machine Wizard.

**Step 07** - Then the virtual machine will appear as shown as below.

![](http://i.imgur.com/FCQxuVh.png)


![](http://i.imgur.com/gm7Oqei.png)


![](http://i.imgur.com/ic62qWN.png)


![](http://i.imgur.com/w4qkkld.png)


![](http://i.imgur.com/DIX5Qac.png)

**Step 08** - Press "Enter" key to continue the VMware ESXI 5.5.0 installation.
 
![](http://i.imgur.com/A33GslR.png)

**Step 09** - Then accept the End User License Agreement by pressing "F11" key.

![](http://i.imgur.com/8Ic1NY1.png)
 

**Step 10** - Then it will scan for available devices. This will take few time.

**Step 11** - Continue Select a Disk to Install or Upgrade by pressing "Enter" key.

![](http://i.imgur.com/e0rE8o2.png)

**Step 12** - Then continue the installation by following given instructions on each and every window.

* Press "Enter" key to select a keyboard layout.

![](http://i.imgur.com/bQratVh.png)

**Step 13** - Provide a root password and confirm it. Make sure to remember this password.Then press "Enter" key.

![](http://i.imgur.com/HyJKFkt.png)

**Step 14** -Then it will scan the system.This will take few time.

![](http://i.imgur.com/yt2lIVZ.png)

**Step 15** - Now confirm install by pressing "F11" key.

![](http://i.imgur.com/jJ8zVxu.png)

**Step 16** - It will start installing ESXI 5.5.0 as shown as below screen shot.It takes some time to install ESXI 5.5.0.

![](http://i.imgur.com/OMstrBC.png)

**Step 17** - Now the installation has been completed. Press "Enter" key to reboot the server.

![](http://i.imgur.com/s4BHrQJ.png)

![](http://i.imgur.com/gOkB1TF.png)

![](http://i.imgur.com/r61gRKL.png)

![](http://i.imgur.com/tw6Ut6z.png)

**Step 18** - It will display DHCP IP address on the screen. 

![](http://i.imgur.com/cb8NQ4U.png)

**Step 19** - Open command prompt application in your host OS.

<pre>PROMPT-> ping IP address</pre>

Example:-
 >  PROMPT-> ping 192.168.220.128

![](http://i.imgur.com/DlvHpWY.png)

**Step 20**- Now download the VMware vSphere client 5.5 by typing, 

<pre>https://Given IP address</pre> in the web browser. It will start downloading shortly.To complete the download it will take a considerable amount of time.

Example :-

![](http://i.imgur.com/4jeQgfU.png)

![](http://i.imgur.com/I43prb6.png)

**Step 21**- After Download completes click on "Open" button

![](http://i.imgur.com/Zr6ndUL.png)

 or if you have already downloaded VMware vSphere client 5.5, 

<pre>Double click on it</pre>
 
![](http://i.imgur.com/HvusrK6.png)

**Step 22**-

* Then it will display,

![](http://i.imgur.com/mJxzBu0.png)

* Now it is displaying, 

![](http://i.imgur.com/uWC5Ofi.png)

on the screen.

* Accept the license agreement. Click on "Next" button.

![](http://i.imgur.com/ds7h5oK.png)

* Select a folder to install VMware vSphere client 5.5. Click on "Next" button.

![](http://i.imgur.com/TeAaJ16.png)

* Click on "Install" button.

![](http://i.imgur.com/5g2KC3Q.png)

**Step 23**- Since I have 4GB RAM in my physical machine I have faced some problems when I work with virtual machine which is already consuming 4GB RAM.
Previously I have done this lab with my colleagues as a collaborative work. Therefore as a solution for that problem I'll put those screen shots from this onward in this report.

* In this window it will ask for IP address, User name and Password. Provide the IP address which you obtain in Step 18. Type the root password which you gave in Step 13. Then click on "Login" button.

![](http://i.imgur.com/Fs0vvDy.png)

* Ignore the security warning.

![](http://i.imgur.com/l8EzJ01.png)

**Step 24**- Now it is possible to view the vSphere Client interface.

![](http://i.imgur.com/VeO28l6.png)

**Step 25**- There are 9 tabs which contains information about the vSphere Client. Click on those tabs and view their details.

**Step 26**- Go to the Summary tab.
<pre> Right click on datastore1 which exists under Storage -> Browse Datastore </pre>

![](http://i.imgur.com/fZkKR2g.png)

**Step 27**- Then select "Upload File" under the forth icon in Datastore Browser-[datastore1] window. 

![](http://i.imgur.com/UJwfr7I.png)

**Step 28**- Select "kali-linux-2.0-amd64.iso" in Upload Items window.

![](http://i.imgur.com/wa265zP.png)


**Step 29**- Then it will upload the file.

![](http://i.imgur.com/mM4577m.png)

**Step 30** - Then it will display "kali-linux-2.0-amd64.iso" in right side of the Datastore Browser-[datastore1] window.

![](http://i.imgur.com/ucAkIJI.png)

**Step 31** - Now, <pre> Right click on IP address -> New Virtual Machine </pre>

![](http://i.imgur.com/aJcJ9jJ.png)

**Step 32** - It will appear the Create New Virtual Machine window.

* Select "Typical" as configuration in Create New Virtual Machine window. Click on  "Next" button. 

  ![](http://i.imgur.com/oM5xZQi.png)

* Give a suitable name for the New Virtual Machine. Click on "Next" button.

![](http://i.imgur.com/GUtpuBb.png)

* Keep datastore1 storage as it is. Then continue by pressing "Next" button.

![](http://i.imgur.com/y5k42lp.png)

* Specify "Linux" as Guest Operating System. Click on "Next" button.

![](http://i.imgur.com/jN6nrVi.png)

* Select "E1000" as Network Adapter. Click on "Next" button.

![](http://i.imgur.com/qTyHucV.png)

* Select "Thin Provision" and click "Next".

![](http://i.imgur.com/AGgtVb2.png)

* Finish creating New Virtual Machine by clicking "Finish".

![](http://i.imgur.com/ZvGYWLg.png)

**Step 33**- Then,
 <pre> Right click on Kali linux -> Edit settings</pre>

![](http://i.imgur.com/LgHbpJo.png)

**Step 34**- Select CD/DVD drive 1 in Virtual Machine Properties window. Click on "OK" button.

![](http://i.imgur.com/XrSanO9.png)

**Step 35**- Now,
<pre>Browse Datastore ISO file</pre>

* Click on check box related to "Connect at power on".

![](http://i.imgur.com/gOJT649.png)

**Step 36**- Then it will appear the newly created virtual machine. Then power on the virtual machine.  

![](http://i.imgur.com/q2vzTd5.png)

**Step 37**- Then it will appear the new kali virtual machine.

![](http://i.imgur.com/jrDzv6s.png)

**Step 38**-

![](http://i.imgur.com/LdrcK6v.jpg)

**Step 39**- Use some commands.

![](http://i.imgur.com/zTfXWAg.png)

![](http://i.imgur.com/1Ihre38.png)

**Step 40**- 

![](http://i.imgur.com/IXHP4uN.jpg)

**Step 41**- Power off the virtual machine.

![](http://i.imgur.com/leDFrCs.png)

![](http://i.imgur.com/paBz9ro.png)

**Step 42**- Finally it will look like this.

![](http://i.imgur.com/FSzdlQH.png)