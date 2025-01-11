
<h1>Digital Imaging With dd: USB Backup And Resoration</h1>


<h2>Description</h2>
This project demonstrates the process of creating a digital image backup of a USB stick and restoring it using the dd command in Linux. The primary purpose is to showcase how disk imaging can be applied across various types of secondary storage, such as hard drives, SSDs, memory cards, and other external storage devices, in addition to USB sticks. This technique is essential in digital forensics and data recovery to preserve and manage data integrity. 

- Key Objectives:

  - Data Preservation: Learn how to create an exact byte-for-byte replica of a USB drive. This is essential in scenarios where data integrity is critical, such as forensic investigations or before performing high-risk operations.
  
  - Recovery and Restoration: Understand how to use the image file to restore the original content of the USB stick, enabling the recovery of lost or corrupted data with minimal hassle.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Bash</b> 
- <b>dd</b>

<h2>Environments Used </h2>

- <b>Kali Linux</b>
- <b>Windows 10</b>

<h2>Walk-through:</h2>
<br>
<br>
<p align="left">
<b> The following screenshot displays the disk and its contents in Windows. For this project, I am utilizing a 1GB USB stick formatted with the FAT32 file system, which contains five files.<b/>
<br>
<br>
  <img src="https://i.imgur.com/60zOPia.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<b> This screenshot demonstrates the creation of a digital image file named imagefat32backup.raw using the dd command in Linux. The command used is sudo dd if=/dev/sdb of=./imagefat32backup.raw bs=1M conv=sync,noerror. Here, /dev/sdb represents the USB stick being imaged, located in the system's /dev directory. You can identify your USB device by running the fdisk -l command. The if= argument specifies the input file or device, while of= defines the output destination and filename for the image. <b/> 
<br>
<br>
  <img src="https://i.imgur.com/AYBBaKg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<b> In this step, I reformatted the USB stick to the FAT-32 file system, effectively clearing its contents. As shown in the following screenshot, the USB stick is now empty and ready for further operations. <b/> 
<br>
<br>
  <img src="https://i.imgur.com/n5aU4nE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<b> The following command demonstrates the process of restoring the USB stick by simply swapping the input (if) and output (of) files from the backup image.<b/> 
<br>
<br>
  <img src="https://i.imgur.com/zhrjbXG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<b> The screenshot shows the successful restoration of files to the USB stick, verified by running the ls command in Linux and viewing the file directory in Windows. <b/> 
<br>
<br>
  <img src="https://i.imgur.com/OSx4BPi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
  <img src="https://i.imgur.com/I1OIFNY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
