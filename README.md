 <h1>Implementing Vulnerability Management Functions On Sandbox Networks</h1>

 ### 

<h2>Description</h2>
In this project we will address vulnerability scanning and remediation, essential steps in the Vulnerability Management Lifecycle. Nessus Essentials will be utilized to scan local VMs hosted on VMWare Workstation. The process involves running credentialed scans to identify vulnerabilities, addressing some of them through remediation, and conducting a follow-up rescan to verify the effectiveness of the remediation. 
<br />


<h2>Utilities Used</h2>

- <b>Nessus Essentials</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (22H2)

<h2>Program walk-through:</h2>

To begin, let's download VMware for Windows. 

[Download: VMware](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) <b><i></b></i>
             
[Download: Windows 10 ISO](https://www.microsoft.com/en-us/software-download/windows10) <b><i></b></i>  
<br /> 
[Download: Nessus Essentials](https://www.tenable.com/products/nessus/nessus-essentials) <b><i></b></i>                                                                                                                        <br />
<br /> 
 While VMware is downloading, head over to Windows and download the ISO as well. 
                                                                                      <br/>
                                                                                      <br />
<img src="https://i.imgur.com/OJn65Y9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
              <br/>

   <br />
<img src="https://i.imgur.com/9wAYXgk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />

<br />
Once the Windows tool is downloaded, open it up and accept the terms, and click "Create installation media" since we need the ISO file.                                   <br/>
                                   <br />
<img src="https://i.imgur.com/WaWgDIV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />


<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/MvTXdP1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />


<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/BSiHR8e.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />



<br />
<br />
Be sure to select ISO file and click next. Make a note of where you download it, we will need it in a bit.    <br/>
                                      <br />
<img src="https://i.imgur.com/s3o479K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/ZsOnVQN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<br />
 Now, head over to Nessus Essentials and sign up and click download after signing up.                                     <br/>
                                      <br />
<img src="https://i.imgur.com/Eq8qrLz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
After clicking download, select the options below and click download again. Make note of where you download this as well.                                         <br/>
                                      <br />
<img src="https://i.imgur.com/TuIrAM1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
Once downloaded, open the Tenable Nessus installer and install it.     <br/>
                                      <br />
<img src="https://i.imgur.com/ZZ5qWck.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/n99VW3P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/RxZoLNt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/9STrE0V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
Once installed it should open a browser window. Make a note of the URL as well.    <br/>
                                      <br />
<img src="https://i.imgur.com/skHGvps.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
Then click on "Connect via SSL". Then click advanced, then proceed to localhost (unsafe). You'll then land on a page that looks like this. This will take a little while.      <br/>
                                      <br />
<img src="https://i.imgur.com/qSIz0ag.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>



<br />
<br />
Once completed, select the option below.                                      <br/>
                                      <br />
<img src="https://i.imgur.com/VW8Vl38.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
 On this next part, select skip and enter the activation code that was sent to your email when you signed up.                                     <br/>
                                      <br />
<img src="https://i.imgur.com/WxtQ5AB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/taqUXsF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
 Set up a username and password. Make sure not to forget it!                                    <br/>
                                      <br />
<img src="https://i.imgur.com/VqHZRH4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>



<br />
<br />
 This part will take a while, so go get some coffee and relax!                                      <br/>
                                      <br />
<img src="https://i.imgur.com/CWlgyp9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
While that's finishing up, let's open VMware and create a new VM.                                      <br/>
                                      <br />
<img src="https://i.imgur.com/Tne0J7y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />

<br />
<br />
 Click browse and select the Windows 10 ISO and click next.                                   <br/>
                                      <br />
<img src="https://i.imgur.com/CTswtVg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
Name the VM something easy and leave the location default and click next.                                      <br/>
                                      <br />
<img src="https://i.imgur.com/I92Mh1V.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>



<br />
<br />
Click customize hardware.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/Fnh4VcY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
Make sure to change your VM to the same specs as below.                                     <br/>
                                      <br />
<img src="https://i.imgur.com/FqDTwPv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />

<br />
<br />
Then just make sure that "Power on this virtual machine after creation" click finish.                                    <br/>
                                      <br />
<img src="https://i.imgur.com/7UP804P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
 After it's created, it's going to launch and it will show this screen, press any key to boot up into the Windows ISO.                                     <br/>
                                      <br />
<img src="https://i.imgur.com/XLAvnVn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
Then follow the steps to install Windows.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/S3Pr4Hq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/S5w8Rg3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/ydFAtYb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />

<br />
<br />

<br />
<br />
Accept the terms and click custom.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/YEBKYIf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/oOl1zOH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/4td2jyk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/PIwUNLU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                    <br/>
                                      <br />
<img src="https://i.imgur.com/KIJrGXG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/jtz8xM9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/tYp0HyY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/PFnxGTF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/T9Asw7g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/o3K0zo5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
 Name it whatever you'd like, I named it Admin to make it simple.                                      <br/>
                                      <br />
<img src="https://i.imgur.com/qb6vn16.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/GEli2aT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/xDGdD6E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Select no to all of the options.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/lF6b3Wp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />


<br />
<br />
Click not now.                                    <br/>
                                      <br />
<img src="https://i.imgur.com/WpfKGk4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
 Now we'll go to the VM and get the IP. Open your VM and open CMD and type ipconfig just to get the IPV4 Address.                                    <br/>
                                      <br />
<img src="https://i.imgur.com/r1sndX8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
Then disable the firewall (NEVER DO THIS IN PRODUCTION HOME LAB ONLY) go to start>type wf.msc>Windows defender firewall properties. <br/>
                                  
  <br />
<img src="https://i.imgur.com/qm1v0yz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Turn off the first 3 tabs.            <br/>
                                      <br />
<img src="https://i.imgur.com/Xpa7Hd5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
Then open CMD on your own computer and try to ping your VM.                                      <br/>
                                      <br />
<img src="https://i.imgur.com/3o4PU1N.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Now, head back over to Nessus Essentials and in the top right corner click "new scan" and then "Basic Network Scan"                                        <br/>
                                      <br />
<img src="https://i.imgur.com/YOxPYNm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
Name it whatever you'd like and paste the IP Address of your VM and click save.                       <br/>
                                      <br />
<img src="https://i.imgur.com/n4y7MLS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Once saved, click launch to begin the scan. This first scan we are doing is without credentials so we shouldn't expect to see that much of what might actually be vulnerable. We'll do that scan a little later.                                   <br/>
                                      <br />
<img src="https://i.imgur.com/0h9lryT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br /> In your VM, open services. and enable remote registry. This allows the scanner to connect to your VM's registry and look for insecure configurations etc. Change the settings to match the image below and then click apply and start.   <br/>
                                      <br />
<img src="https://i.imgur.com/wh97doX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Now go to user account control settings and drag to never notify.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/QY8sfiY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />


<br />
<br />
 Then go to Registry, follow the path and right click and create a new DWORD labeled Local Account Token Filter Policy and add 1 to the value and restart the VM.                                    <br/>
                                      <br />
<img src="https://i.imgur.com/CsfFlqs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Now head back over to Nessus Essentials, check the box of your VM and in the top right corner click more then configure then click the credentials tab then click Windows and add your admin account. Once added, launch scan.      <br/>
                                      <br />
<img src="https://i.imgur.com/HGlyqpG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
 As you can see, the 2nd scan has a lot more vulnerabilities when comparing it to the 1st scan.                                      <br/>
                                      <br />
<img src="https://i.imgur.com/ef6BbOR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
 The reason is because the credential scan has the ability to scan file systems, the Registry and any other running services.                                     <br/>
                                      <br />
<img src="https://i.imgur.com/7tHhkDU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
Now let's take a look at the vulnerabilities tab. Nessus shows you which vulnerabilities are the most important in regards to priority and it also shows you the detail of the threat and the possible solution.                                      <br/>
                                      <br />
<img src="https://i.imgur.com/Q75dHFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
If you click on remediations, it will give you high level instructions on how to remediate most of the findings.                                     <br/>
                                      <br />
<img src="https://i.imgur.com/PAphWho.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
Before we remediate the findings, we are going to install an old version of Firefox and run another scan to see the vulnerabilities it has. So go to your VM and go to Google and search old versions of Firefox and download and install it and click finish. Below is what I just happen to install. Once that's done, open Nessus and launch another scan.                                    <br/>
                                      <br />
<img src="https://i.imgur.com/jbuRK5A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Looks like the scan picked up the old Firefox that we downloaded and as you can see, it has so many vulnerabilities. Now we can remediate some of the findings. I'm going to uninstall Firefox and then check for Windows updates since that will fix the majority of the issues then we can run a final scan and see the results.                                                                  <br/>
                                      <br />
<img src="https://i.imgur.com/cuetEuE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/zLej1Wx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
Ok, So I uninstalled Firefox and did some Windows updates and it looks like Windows is up to date, now lets run our final scan and see the results.                                      <br/>
                                      <br />
<img src="blob:https://imgur.com/925ff33c-003f-410f-890f-74f1573ff14d" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />


<br />
<br />
Final scan results.                                     <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />


<br />
<br />
                                    <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />


<br />
<br />
                                    <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />


<br />
<br />
                                    <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />


<br />
<br />
                                    <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />

<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
                                      <br/>
                                      <br />
<img src="" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />



