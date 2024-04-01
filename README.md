<h1>Mastering Heavy Forwarder Configuration in Splunk: A Step-by-Step Guide for Beginners</h1>
Configuring a heavy forwarder in Splunk involves setting up the forwarding and receiving of data between different components within the Splunk ecosystem. This process requires configuring receiving ports on indexers and search heads, establishing forwarding settings on the heavy forwarder, applying appropriate licensing, and directing data flow efficiently. With a heavy forwarder properly configured, organizations can seamlessly forward, monitor, and manage data across their Splunk environment, facilitating effective analysis and decision-making.
<br />

<h2>Requirements</h2>
- Splunk Software</b> 

<h2>Execution Steps</h2>
Configure Receiving on Indexers and Search Head:
Navigate to "Settings" and proceed to "Forwarding and Receiving".



<p align="center">
<img src="https://imgur.com/VT4rLzp.png" height="80%" width="80%" alt="Disk Sanitization 
 Steps"/>
<br />
<br />
 
Initiate the configuration of receiving by selecting the appropriate option.
<p align="center">
<img src="https://imgur.com/77ksIve.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br /> 
 
Within the receiving configuration, locate the option to create a new receiving port.

<p align="center">
<img src="https://imgur.com/JulUw3M.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
 
Input the default receiving port, typically "9997", or specify a port of your choice. Save the settings upon completion.

<p align="center">
<img src="https://imgur.com/Fggrw0S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Configure Forwarding on Heavy Forwarder:
•	Return to "Settings" and access "Forwarding and Receiving" once more.


<p align="center">
<img src="https://imgur.com/wlaLBgi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
  
This time, focus on configuring forwarding and applying a forwarding license

<p align="center">
<img src="https://imgur.com/ynkEQUJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
  
Add New Forwarding Host:
•	Choose the option to add a new forwarding host.

<p align="center">
<img src="https://imgur.com/pMMqQxq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Enter the host IP address or hostname along with the designated port. You can determine the IP address using the command "ip addr" on your server as shown in the second image. Save the settings to activate forwarding.

<p align="center">
<img src="https://imgur.com/w4I03ZL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
<img src="https://imgur.com/LGSBbyv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
<img src="https://imgur.com/ozhitrl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Apply Forwarding License:
•	Navigate to "Settings" and select "Licensing".

<p align="center">
<img src="https://imgur.com/onT5TB2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

•	Opt to change the licensing group and choose the forwarder license. 

<p align="center">
<img src="https://imgur.com/iH2hJh5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

•	Save the changes and restart Splunk to apply the license.

<p align="center">
<img src="https://imgur.com/GPH1lBS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Forward Data and Monitor Directory: After restarting, proceed to "Settings" once more and select "Add Data".

<p align="center">
<img src="https://imgur.com/M0hlzrL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Now monitor your directory on the forwarder.


<p align="center">
<img src="https://imgur.com/7u5KD9x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

 
Choose "Files and Directories

<p align="center">
<img src="https://imgur.com/fGTg5be.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Now browse the files system.

<p align="center">
<img src="https://imgur.com/8ln8ZZZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

select the desired file

<p align="center">
<img src="https://imgur.com/qdC6EhV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Go to next

<p align="center">
<img src="https://imgur.com/NkJAXc0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Proceed through the configuration steps, leaving settings at default unless adjustments are necessary based on specific requirements 

<p align="center">
<img src="https://imgur.com/upaNL5E.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

Review and submit the configuration.

<p align="center">
<img src="https://imgur.com/EMe9oT9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

As the heavy forwarder is primarily for forwarding data, you won't be able to perform searches directly on it


<p align="center">
<img src="https://imgur.com/cz7bony.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


Navigate to the "Search and Reporting" app from the home screen.

<p align="center">
<img src="https://imgur.com/dHkIruT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


In the search field, input "host=splunkhf". Adjust the time range to "All Time" and execute the search to verify data forwarding from the heavy forwarder (hf).

<p align="center">
<img src="https://imgur.com/SXyJCiS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">
<img src="https://imgur.com/A11GJuc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
