![image](https://github.com/Naeshon/creating-vms/assets/153772720/1b8f1446-e597-4acc-8048-da5a125e50f2)






<h1>Creating a Virtual Machine & Logging Into It Through Remote Desktop in Windows (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
  

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Virtual Machine Creation & Configuration Steps</h2>

- Log into your Microsoft Azure account
- Set up the Virtual Machine
- Find the VM's Public IP & Connect through Remote Desktop
  

<h2>Configuration Steps</h2>

![image](https://github.com/Naeshon/creating-vms/assets/153772720/5604868e-010b-47b1-91a1-d69cc3f7917b)

<p>
1) Once you've logged into your Azure account, navigate to the home panel and find the button that says 'Virtual Machines', if you cannot find it you can also search for it at the top of the screen.
</p>
<br />


![image](https://github.com/Naeshon/creating-vms/assets/153772720/ea7d663a-7cdb-4ab4-a8ed-3760000bbd98)


</p>
<p>
2) From this screen you may click create, then Azure virtual machine.
</p>
<br />

![image](https://github.com/Naeshon/creating-vms/assets/153772720/c47caf5f-3dff-4e14-8ae7-4c98ee2c52b0)

<p>
3) Now we may configure the basic settings such as selecting the operating system that the VM will use, in this case I will choose Windows 10. Make sure the VM is big enough to run windows without a problem, I would recommend atleast 2vcpu's just so the VM is capable of running everything smoothly (you will also need to create a login name & password that you will need later to log into the VM through Remote Desktop).
</p>
<br />


![image](https://github.com/Naeshon/creating-vms/assets/153772720/fd3dcd2d-08eb-48f7-92e0-26073a8a0c02)

4)This step is unnecessary for this example but if you wanted to make 2 VM's and connect them to the same network you would have to connect the second VM to the same virtual network as the first one & also make sure they are both located in the same Resource Group in Azure. But for this exercise we will just create a new virtual network for the VM to connect to. If everything looks good we can hit 'Review + Create' and wait for validation to pass. Once the validation has passed we will be able to click create & wait for the deployment, this will take a couple minutes.

![image](https://github.com/Naeshon/creating-vms/assets/153772720/ac7ca514-a530-4b35-8fca-25bb55415ad9)

5) Once the deployment is complete we can click 'Go To Resource' to get to the VM Overview page, this is where the Public IP Address is found, we will use this adrress in Remote Desktop to find our VM.

![image](https://github.com/Naeshon/creating-vms/assets/153772720/9cc32edd-0049-493b-8a3f-8da593b9f7a5)

6) Now we can open Remote Desktop Connection and enter our Virtual Machines public IP address.

