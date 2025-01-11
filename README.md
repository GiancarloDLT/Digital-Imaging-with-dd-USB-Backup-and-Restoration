# Digital-Imaging-with-dd-USB-Backup-and-Restoration

<h1>Digital Imaging With dd: USB Backup And Resoration</h1>


<h2>Description</h2>
This project demonstrates the process of creating a digital image backup of a USB stick and restoring it using the dd command in Linux. The primary purpose is to showcase how disk imaging can be applied across various types of secondary storage, such as hard drives, SSDs, memory cards, and other external storage devices, in addition to USB sticks. This technique is essential in digital forensics and data recovery to preserve and manage data integrity. 

- Key Objectives:

  - Data Preservation: Learn how to create an exact byte-for-byte replica of a USB drive. This is essential in scenarios where data integrity is critical, such as forensic investigations or before performing high-risk operations.
  
  - Recovery and Restoration: Understand how to use the image file to restore the original content of the USB stick, enabling the recovery of lost or corrupted data with minimal hassle.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Bash</b> 
- <b>xxd</b>
- <b>[Gary Kessler's Website](https://www.garykessler.net/library/file_sigs.html)</b>

<h2>Environments Used </h2>

- <b>Kali Linux</b>

<h2>Walk-through:</h2>
<br>
<br>
<p align="left">
<h3> In this section, we will explore the file signatures of the "cat.jpg" image:</h3>
<br>
<br>
  <img src="https://i.imgur.com/AjYToXE.jpeg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<b> The following screenshot comes from Gary Kessler's Website, showcasing the header (FF D8) and trailer (FF D9) of a JPG file.<b/> 
<br>
<br>
  <img src="https://i.imgur.com/GwUqRs3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
