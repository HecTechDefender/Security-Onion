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

To begin, let's download Vmware for Windows. 

[Vmware](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) <b><i></b></i>
                
<br />
<br />
 While Security Onion is downloading, head over to VirtualBox and download that as well. 
                                                                                      <br/>
                                                                                      <br />
<img src="https://i.imgur.com/M7PCKZb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
               <br/>

  <br/>
                                    <br />
<img src="https://i.imgur.com/wLOK7f8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />

<br />
 Install and leave everything default.                                     <br/>
                                   <br />
<img src="https://i.imgur.com/gg5PlJb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />


<br />
This window is simply informing you that if you click on it, your network adapters/network connections will be disconnected. To be safe, make sure that Security Onion has finished downloading before continuing. If it's already downloaded, click yes.  <br/>
                                      <br />
<img src="https://i.imgur.com/YQ94f0u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

<br />


<br />
If you haven't installed VirtualBox before, there will be some dependencies, no need to worry, this window will auto install those dependencies for you so just click install.        <br/>
                                      <br />
<img src="https://i.imgur.com/8hJ9Sno.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />



<br />
<br />
While that's installing, go back to the Security Onion github page and cross reference the file hash numbers (highlighted SHA256 number) and make sure they match to ensure that they didn't get tampered with while downloading. 

To check the file hash of Security Onion, open the folder where it is downloaded and hold SHIFT + RIGHT CLICK on the mouse and click "Open PowerShell window here" then type Get-FileHash SecurityOnion hit TAB and press ENTER. It should reveal the file hash number.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/DOG0ZAs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
 Once all that's verified, open VirtualBox and click on "new".  Name your new machine "Security Onion" and then select the Security Onion ISO file. Then check the box "Skip Unattended Installation".                                      <br/>
                                      <br />
<img src="https://i.imgur.com/rCzPDlp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<br />
Make sure to select the minimum requirement for Security Onion: 16GB RAM & 2 processors.     <br/>
                                      <br />
<img src="https://i.imgur.com/6GZBj5Q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br /> In regards to storage, Security Onion recommends 200GBs, but it's up to you.                                        <br/>
                                      <br />
<img src="https://i.imgur.com/iqfhvty.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
 On this last page, just make sure everything looks correct and then click finish.    <br/>
                                      <br />
<img src="https://i.imgur.com/MK2dkxH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
Then click start to open your new virtual machine. Once opened, it will look like this. Type the entire word "yes" to proceed. Then create a username and enter a admin password, hit enter and let it do it's thing. After installation, it will ask you to press enter to reboot!                <br/>
                                      <br />
<img src="https://i.imgur.com/IW7Gw8m.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>

  
<br />
<br />
 Once that's done, you'll land on a log on page. Enter the username and password that you entered just a bit ago.  Then you'll be presented with a set up page. Click yes.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/xFVEDzI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/17pfOHk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/jn3cmze.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>


<br />
<br />
 Type "AGREE"                                    <br/>
                                      <br />
<img src="https://i.imgur.com/8T4QjYl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br/>



<br />
<br />
                                      <br/>
                                      <br />
<img src="https://i.imgur.com/kO6zaa5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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


