
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
###AWS Instances Summary Report###
</center>

----------

####Name :  Perera K. A. U####
####SLIIT ID :  IT13019600####
####AWS username :  Achini####
####Practical Session: WD (Friday 3.30 pm- 5.30 pm)####


----------
----------
####Practical Number: Lab 01####
####Practical Title: Creating an Amazon EBS-Backed Windows AMI####
----------
----------
<br>
</br>

**Step 01** – First, create an AWS account by providing relevant details.


**Step 02** – Then need to sign in to Amazon Web Services by providing a valid E-mail and a password. Now click on “Sign in using our secure server” button.

![](http://i.imgur.com/0k3J50A.png)


<br>

</br>
**Step 03** – Click EC2 link.
<br>

![](http://i.imgur.com/AhO2pUD.png)


</br>

**Step 04** –To launch an Amazon EC2 instance, click on “Launch Instance” button.

![](http://i.imgur.com/UzGSIIs.png)

<br>

</br>
**Step 05**– Choose an Amazon Machine Image (AMI). Select Microsoft Windows Server 2012 R2 Base. Click on “Select” button.

![](http://i.imgur.com/qZ7rwpl.png)
<br>

</br>

**Step 06** – Choose t2 micro (Free tier eligible) instance as instance type. Click on “Review and Launch” button.

![](http://i.imgur.com/Tc13Vix.png)

<br>

</br>
**Step 07** – Then Review instance launch details. Click “Launch” button to complete the launch process.

![](http://i.imgur.com/HTuY1Yk.png)
<br>

</br>

**Step 08** – Then to complete the launch process “Selecting an existing key pair or create a new key pair” window appears. Select “Create a new key pair” from drop down list and give a name for key pair. Then click on “Download Key Pair” button. Now click on “Launch instances” button.

![](http://i.imgur.com/wYRvuDh.png)

<br>

</br>
**Step 09**– Then the Key pair will be downloaded. The extension is .pem and now instances are launching. Click on the instance code.

![](http://i.imgur.com/VQHzZd1.png)
<br>

</br>

**Step 10** – The instance details are shown in the window. The instance’s state will become to running state shortly. 

![](http://i.imgur.com/leZlNws.png)

<br>

</br>
**Step 11** - Now click on “Connect” button.

![](http://i.imgur.com/rkzScV1.png)
<br>

</br>

**Step 12** – In order to connect to the instance username and password are needed. Click on “Get Password” button.

![](http://i.imgur.com/irrdxRJ.png)

<br>

</br>
**Step 13** - So browse the .pem file which was downloaded at the beginning and click on “Decrypt Password” button.

![](http://i.imgur.com/FhhVpZg.png)
<br>

</br>

**Step 14** – Here copy and paste this Public DNS and Password somewhere future use. Then click on “Download Remote Desktop File” button to download the remote desktop file. Now click on “Close” button.

![](http://i.imgur.com/litFAju.png)

<br>

</br>
**Step 15** – It will download the file. Then Run it. IT will appear the “Remote Desktop Connection” window. Click on “Connect” button.

![](http://i.imgur.com/y152DoK.png)
<br>

</br>

**Step 16** – Enter the password which was saved in Step 12 as the Administrator password. Then click on “OK” button.

![](http://i.imgur.com/EcWrYME.png)

<br>

</br>
**Step 17** – Click on “Yes" button in this window.

![](http://i.imgur.com/X1cn3PR.png)
<br>

</br>

**Step 18**- It will initialize the remote desktop connection.

![](http://i.imgur.com/XlDkPbu.png)

<br>

</br>

**Step 19** – Now can get the Microsoft Windows Server 2012 R2. This virtual server can be used for working purposes. 

![](http://i.imgur.com/H5rQ9Du.png)
<br>

</br>

**Step 20** – Do some work.

![](http://i.imgur.com/XC0iFVV.jpg)

<br>

</br>

**Step 21** – After finishing the work close it.

![](http://i.imgur.com/lfEMKtA.png)


<br>

</br>
**Step 22** - Even after the closing, the instance is still running. To terminate it,
<pre> Right click on the instance -> Instance State -> Terminate</pre>

![](http://i.imgur.com/0svq2hY.png)
<br>

</br>

**Step 23**– Confirmation to terminate. Click on “Yes, Terminate” button.

![](http://i.imgur.com/6tIPWqf.png)

<br>

</br>
**Step 24**– Now the instance is in Shutting-down state. It will become Terminated state shortly.

![](http://i.imgur.com/E8aWlJU.png)

<br>

</br>

**Step 25** – Now the instance is in Terminated state.

![](http://i.imgur.com/Fsg9jbc.png)

<br>

</br>
----------
----------
####Practical Number: Lab 02####
####Practical Title: Creating an Amazon Linux AMI######
----------
----------
<br>

</br>

**Step 01**– Sign in to AWS account by providing a valid E-mail and a password. Now click on “Sign in using our secure server” button.

**Step 02**– Click EC2 link.
<br>

</br>

**Step 03** –To launch an Amazon EC2 instance, click on “Launch Instance” button.

![](http://i.imgur.com/CzMIWgM.png)

<br>

</br>
**Step 04** – Choose an Amazon Machine Image (AMI). Select Amazon Linux AMI 2016.03.3 (HVM), SSD Volume Type or Red Hat Enterprise Linux 7.2. HVM), SSD Volume Type Click on “Select” button.

![](http://i.imgur.com/k9dGMjf.png)
<br>

</br>

**Step 05** – Choose t2 micro (Free tier eligible) instance as instance type. Click on “Review and Launch” button.

![](http://i.imgur.com/ImzcIPE.png)

<br>

</br>

**Step 06**– Then Review instance launch details. Click “Launch” button to complete the launch process.

![](http://i.imgur.com/NTaFHmY.png)
<br>

</br>

**Step 07** – Then to complete the launch process “Selecting an existing key pair or create a new key pair” window appears. Select “Create a new key pair” from drop down list and give a name for key pair. Then click on “Download Key Pair” button. Now click on “Launch instances” button.

![](http://i.imgur.com/HVeOmbV.png)

<br>

</br>
**Step 08** – Then the Key pair will be downloaded. The extension is .pem and now instances are launching. Click on the instance code.

![](http://i.imgur.com/U4HbnIM.png)
<br>

</br>

**Step 09** – The instance details are shown in the window. The instance’s state will become to running state shortly. 

![](http://i.imgur.com/tDeTOu3.png)

<br>

</br>
**Step 10**- In here it is different from Windows virtual server. Now download “Putty” application from link in below screenshot. Click on putty.exe and puttygen.exe links.

[http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html)
<br>

</br>

**Step 11**– Then double click on puttygen.exe to run it. It looks like this. Now click on “Run” button.

![](http://i.imgur.com/6u8WUOi.png)

<br>

</br>
**Step 12**– Putty Key Generator window appears as shown as below screenshot.

![](http://i.imgur.com/sDgxWLS.png)
<br>

</br>

**Step 13**– Then load the .pem file which was downloaded at the beginning after click on “Load” button.

<br>

</br>

**Step 14**– Click on “OK” button and “Save private key” button in Putty Key Generator interface.

![](http://i.imgur.com/4AmXum0.png)

**Step 15**– Then click on “Yes” button.

![](http://i.imgur.com/QO6hRLn.png)

<br>

</br>

**Step 16**– Save the key by giving appropriate name. 
<br>

</br>

**Step 17**- Then double click on putty.exe to run it. It looks like this. Now click on “Run” button.

![](http://i.imgur.com/qLavwsm.png)

<br>

</br>
**Step 18**– In Putty Configuration window select,
<pre>SSH -> Auth from category </pre>
<br>

</br>

![](http://i.imgur.com/QD6Yigh.png)
!

<br>

</br>

**Step 19**– Browse and select .ppk file saved in Step 17.

![](http://i.imgur.com/ii7HCNv.png)

<br>

</br>
**Step 20**– Now select Session from category. Copy the Public DNS in Amazon web services page right hand side. Paste it in Host Name field in Putty Configuration window.

![](http://i.imgur.com/tFvlpD7.png)
<br>

</br>
<br>

</br>

**Step 21**–All steps are completed. Now click on “Open” button. Now Linux terminal is launching. Click on “Yes” button in Putty Security Alert window.

![](http://i.imgur.com/5CkNXOk.jpg)


<br>

</br>
**Step 22**– Now type commands that are acceptable in Linux environment and get the output. Examples are shown below.
<pre>(ls –al, date, hostname, uname –a, uptime, w, echo 10+5|bc –l, cal 7 2016, cal 2016)</pre>
<br>

</br>


![](http://i.imgur.com/EwVOOg0.png)

<br>

</br>
**Step 23**– Now to exit, type exit and enter or else close the window. Click on “OK”.

![](http://i.imgur.com/L4FxcYi.png)

<br>

</br>
**Step 24**- Even after the closing, the instance is still running. To terminate it,
   <pre> Right click on the instance -> Instance State -> Terminate </pre>

![](http://i.imgur.com/NdNiCOY.png)
<br>

</br>

**Step 25**- Confirmation to terminate. Click on “Yes, Terminate” button.

![](http://i.imgur.com/7pkDdxJ.png)

<br>

</br>
**Step 26**– Now the instance is in Shutting-down state. It will become Terminated state shortly.

![](http://i.imgur.com/CzyTZje.png)

<br>

</br>

**Step 27**– Now the instance is in Terminated state.

![](http://i.imgur.com/9tjFKtq.png)

<br>

</br>

----------
----------
####Practical Number: Lab 03####
####Practical Title: Creating an Amazon RDS Database######
----------
----------
<br>

</br>
**Step 01**– Sign in to AWS account by providing a valid E-mail and a password. Now click on “Sign in using our secure server” button.

**Step 02**– Click RDS link.

![](http://i.imgur.com/OFBASCY.png)

<br>

</br>
**Step 03**– To launch an Amazon RDS DB instance, click on “Launch a DB Instance” button.

![](http://i.imgur.com/9uQV4Uo.png)
<br>

</br>

**Step 04**- On the Select Engine page, choose the MySQL icon and  click on "Select" button.

![](http://i.imgur.com/eoTNFsE.png)

<br>

</br>
**Step 05**- Click on the radio button which is relevant to MySQL under Dev/Test in production page. Next click on "Next Step" button.

![](http://i.imgur.com/eEpXzg1.png)

<br>

</br>

**Step 06**- On the Specify DB Details page, select relevant DB instance information as follows.

![](http://i.imgur.com/YotYWAF.png)

![](http://i.imgur.com/CwutFvs.png)
<br>

</br>

**Step 07**- On the Configure Advanced Settings page, provide relevant information which are needed to launch the MySQL DB instance.

![](http://i.imgur.com/X1OmL2W.png)

<br>

</br>
**Step 08**- After providing additional details click on "Launch DB Instance" button.

![](http://i.imgur.com/B5Ygesg.png)

<br>

</br>

**Step 09**- To view successfully created DB instance, click on "View Your DB Instance" button.

![](http://i.imgur.com/zEy0UgS.png)


<br>

</br>
**Step 10**- The new DB instance has to pass "creating" and "backing-up" states until the DB instance is created. Endpoint appears from now onward.

![](http://i.imgur.com/HHnR4Ik.png)

<br>

</br>

![](http://i.imgur.com/h6jEpqq.png)

<br>

</br>
**Step 11**- When it becomes ready to use (it takes several minutes to change the state) the state is changed to "available" and now connecting to a database on the DB instance is possible.

![](http://i.imgur.com/Opkr3dZ.png)
<br>

</br>

**Step 12**- Once the Amazon RDS is available, want to use 
any standard SQL client application in order to connect to a database on a MySQL DB instance. 

For example MySQL Workbench or XAMPP control panel can be used. 

<br>

</br>
**Step 13**- In here XAMPP control panel is used. Open up the XAMPP control panel, click on 
<pre> MySQL -> Start -> Shell </pre>
<br>

</br>
![](http://i.imgur.com/OVD97fm.png)
<br>


<br>

</br>
**Step 14**- Type the following command at the command prompt/shell on client computer to connect to a database on a MySQL DB instance. 

Substitute Endpoint mentioned in step 10 and step 11 for "endpoint" and Master Username which provided in step 06 for "masterusername".

<pre>
PROMPT> mysql -h "endpoint" -P 3306 -u "masterusername" -p
</pre>
<br>

</br>

![](http://i.imgur.com/BmV8ZII.png)
<br>

</br>

**Step 15**- After pressing Enter key it'll appear a space to type the password, type the Master Password used in step 06.

It'll display the following output.

<pre>
Welcome to the MySQL monitor.  Commands end with ; or \g.
Your MySQL connection id is 21
Server version: 5.6.19-log MySQL Community Server (GPL)

Copyright (c) 2000, 2013, Oracle and/or its affiliates.All right reserved.

Oracle is a registered trademark of Oracle Corporation and/or its affiliates. Other names may be trademarks of their respective owners.

Type 'help;' or '\h' for help. Type '\c' to clear the current input statement.

mysql>
</pre>
<br>

</br>

![](http://i.imgur.com/BaMH9go.png)

<br>

</br>

**Step 16**- Now create a database by typing below command at shell as shown below. Substitute any database name for "databasename".

<pre>
mysql> create database "databasename";
</pre>

**Step 17**- Then create a table by typing following command,

<pre>
mysql> create table "tablename" ("columnname" "datatype"(length));
</pre>

Substitute relevant names for "tablename", "columnname", "datatype" and provide suitable length.

**Step 18**- After that insert several values to the created table. Command is shown below.

<pre>
mysql> insert into "tablename" ("columnname")
    -> values (value);
</pre>


<br>

</br>
**Step 19**- Now it is possible to view the table with inserted values. Type below command at shell.

<pre>
mysql> select * from "tablename";
</pre>

It'll display the same as following output according to your input details.

![](http://i.imgur.com/ZV9ZUIs.png)


<br>

</br>
**Step 20**- Exit from the shell by typing command as,
<pre>
mysql> exit
</pre>

<br>

</br>


**Step 21**- In order to delete the instance,
<pre> Right click on the instance -> Delete</pre>
<br>

</br>

![](http://i.imgur.com/Bojc2ez.png)
<br>


<br>

</br>
**Step 22**- It'll redirect to Delete DB Instance page. Press "Delete" button.

![](http://i.imgur.com/tupH7Hq.png)
<br>

</br>
<br>

</br>
**Step 23**- The DB instance will be deleted shortly.

![](http://i.imgur.com/iqxtJXe.png)

![](http://i.imgur.com/HJL7ty8.png)
<br>

</br>


**Step 24**- Inside the shell it is needed to provide SQL syntax which are relevant to our MySQL server version. Otherwise it'll give syntax errors as follows.

![](http://i.imgur.com/rqJLuOy.png)
<br>

</br>

----------


