<h1>Implementing Security Onion</h1>

 ### 

<h2>Description</h2>
In this project, we're diving into setting up Security Onion and getting our hands dirty with a practical lab. We'll kick things off with the installation and wrap up by walking through a malicious PCAP. 
<br />


<h2>Utilities Used</h2>

- <b>Security Onion</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (22H2)

<h2>Program walk-through:</h2>

To begin, let's download Security Onion. Make sure to download version: 2.4.40-20240116 ISO image.

[Security Onion](https://github.com/Security-Onion-Solutions/securityonion/blob/2.4/main/DOWNLOAD_AND_VERIFY_ISO.md) <b><i></b></i>
                
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

To check the file hash of Security Onion, open the folder where it is downloaded and hold SHIFT + RIGHT CLICK on the mouse and click "Open PowerShell window here" then type Get-FileHash SecurityOnion hit TAB and press ENTER.  It should reveal the file hash number.                                       <br/>
                                      <br />
<img src="https://i.imgur.com/DOG0ZAs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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


