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
###V-Motion Report###
</center>

----------

####Name :  Perera K. A. U####
####SLIIT ID :  IT13019600####

####Practical Session: WD (Friday 3.30 pm- 5.30 pm)####
####GITHUB URL:####

Markdown file:

PDF file:

----------
----------

####V-Motion migration####

![](http://i.imgur.com/aJGnI1K.jpg)

A v- motion migration moves a powered on virtual machine from one ESXi host to another host without losing service. V-motion simply means, migrating a virtual machine(VM), currently running on a hardware, to another available hardware.

V-motion can be used to :

* Improve overall hardware utilization. Can handle load balancing.

* Allow continued virtual machine operation while accommodating scheduled hardware downtime -> We can't eliminate the hardware downtime. For example, if hardware need to repair, the operating system is not possible to run top of that anymore. Then we can migrate the VM , do necessary changes in the new location and migrate back the VM.The place we are migrating the VM(destination) is a temporary location.

* Allow vsphere Distributed Resource Scheduler(DRS) to balance virtual machines across hosts.


#####Requirements for v-motion

Virtual machine(VM) must meet the following requirements:

* A VM must not have a connection to a virtual device such as a CD-ROM/ floppy drive with a local image mounted -> Some times iso s will be assigned to the local disk. So if we are going to migrate that, it is not possible since it is requested from the same CD ROM. So the operating system/ file should be there in the shared folder. Not in the local storage. It is needed to avoid the dependency between the hardware and software, before migrating.

* A VM must not have a connection to an internal vSwitch.
* A VM must not have CPU affinity configured -> If the operating system cannot run on another CPU/ the operating system requires the same CPU, there is a bond between the operating system and the CPU. Because of affinity it requires the same hardware. If the affinity is configured then v-motion is not possible.

Source and destination host must have:

* Visibility to all storage used by the VM
* At least a Gigabit Ethernet network
* Access to the same physical networks
* Compatible  CPUs
 
##### Necessary components to do a V-motion#####

* V-motion network -> The v-motion network is dedicated only for the virtual matching moving process. There should be a proper network connection in order to VM from one place to another place. the v-motion network should be a high speed network connection than the production network. 

* Production network -> The production network is used for sharing data and information.

* Shared data store -> There should be a common data store for both two VMEXSi s.They both will able to access it.Data store contains hard disk files etc...

Except those three components, we want to move the status also. Status is stored in RAM of a particular machine. It can be either hardware status or software status or CPU status.Moving the status helps to continue the work that we have done in source machine before migration. So there will not be any availability issue. 


At least 12GB RAM is required to do v-motion practically. Since there is only 4GB RAM is in my laptop I am going to describe only the steps below.

**Step 01**- Connect to virtual center and gain access to one of the servers. Select the tab,

<pre>Configuration-> Network Adapters </pre> 
and see the visibility of new connections.

**Step 02**- Look at the tab,

<pre>Configuration-> Networking </pre> and click on "Add Networking" to create the vSwitch. 

**Step 03**- It'll displays the Add Network Wizard. Select "VMKernel" and click on "Next" button.

**Step 04**- Making a network card or cards that have connected from one server to another and clivk on "Next"
button.

**Step 05**- Provide a Network Label as your choice. For example:- Vmotion. Select the check box related to "Use this port group for vMotion" and click on "Next" button.


**Step 06**- Set "Use the following IP setting" as follows.

<pre>IP Address: 50.50.50.2 
(This ip must be different from the server that we configured earlier 1).
Subnet Mask: 255.255.255.252 (Since we will use only 2 ip's).</pre>

Then click on "Next".


**Step 07**- Then click on "Finish". To ensure that the entire system is working properly, migrate a VM from one EXSi to the other using v-motion functionality which you just configured.

Press, <pre> Right mouse button on a virtual machine-> Migrate </pre>

**Step 08**- It'll display Migrate Virtual Machine window. Click on "Next" button.

**Step 09**- Select the target server(destination), where we will move the virtual machine. Then click on "Next" button.

**Step 10**- Click on "Next" button Migrate Virtual Machine (vMotion Priority) window.


**Step 11**- Click on "Finish" to start the migration.





