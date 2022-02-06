# Getting started with **Oracle Linux** 
[Oracle] | [ISO Download] | [Virtualbox Download]

**Below, you will find a detailed walkthrough installation of Oracle Linux in Virtualbox.  This was done using VirtualBox version 6.1.32, and Oracle Linux 8.5 on February 4, 2022. Please [email] me with any questions, concerns, or feedback.** 

`Please note:` *this is with absolute beginners in mind*.


<p align="center">
  <img width="600" height="300" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR_L22k5bcWLXxB9bp446P1u3oCoxIAZj63urWqAOvr2_Q0yW9u1OTBHsX-269NnMP_cQc&usqp=CAU">
</p>

<br />

## Start by downloading the tools:

Locate the appropriate Oracle Linux ISO, [download], for your setup.

Download the latest [virtualbox] binary. _**(Skip if you already have Virtualbox)**_

Install Virtualbox _**(Again, skip if you already have)**_

---
<br />

## Install Oracle Linux in VirtualBox:

You'll want to begin by opening up Virtualbox.  Click **new** as outlined with a *red circle* below.

<p align="center">
<img src="assets/img/1.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>

<br />

I'll be using **Expert Mode** in this installation.

---

## Name and Operating System
- Name: Oracle
    - Name this whatever you like
- Machine Folder: D:\VMs
    - Store your virtual machine in a location that has available space.  In my situation I use a dedicated solid state drive for virtual machines, which is, my D:\ is in this scenario.
- Type: Linux
    - This is a Linux distro
- Version: Oracle(64-bit)
    - This will work if you select other choices; however, Oracle is the version so I do suggest using it.

Memory Size
- Select the amount of memory you are able to dedicate to the virtual machine.  In my case I've selected **8192 mb** which is about *8gb* of memory.

Hard Disk
- For the purpose of this walkthrough, I am, *creating a new virtual disk*.

Click **Create** as outlined in red below.


<p align="center">
<img src="assets/img/2.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

---

## Create Virtual Hard Disk

File Location:
- Ensure this matches the location you would like to store the `virtual disk`.

File Size:
- Set the amount that you are able to allocate to your virtual machine.
    - I selected to use 200gb, but this is for my own use case. **Don't** let this determine your selection.

Hard Disk File Type
- I'm using **VDI**
    - *This may vary for your use case. Refer to documentation regarding questions/concerns*.

Storage on physical hard disk
- I'll be using **Dynamically Allocated**
    - If you have a use case for *Fixed Size* then use that.

Continue by clicking by clicking **Create** after reviewing the information, and ensuring the settings to be satisfactory.

<p align="center">
<img src="assets/img/3.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

---

## Settings

Clicking the gear icon with *"Settings"* under, circled in the photo below in red, will open up the settings of your virtual machine.

<br />
<p align="center">
<img src="assets/img/4.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

## System
We'll start with going into **System** as circled in the image below.

<br />
<p align="center">
<img src="assets/img/5.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

I like to uncheck the floppy and move it to the bottom of the boot order.  It's really just a preference, and not necessary.

Do ensure the memory is what you set earlier, or modify it here while in the **Motherboard** tab.

<br />
<p align="center">
<img src="assets/img/7.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

Next navigate over to the **Processor** tab, as seen below.

<br />
<p align="center">
<img src="assets/img/8.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

I'm able to allocate 4 cores to this virtual machine. You will need to decide on what **CPU** resources to allocate to your virtual machine.  Please read the documentation regarding any questions or concerns here [Oracle]. I make no changes to the execution cap for my use case, and leave the extended features on default settings. If your default settings are different, again, please visit Oracle to locate settings partiuclar to your environment.

<br />
<p align="center">
<img src="assets/img/9.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

## Display 
Next we'll navigate over to the **Display** settings, which I’ve circled in red below.

<br />
<p align="center">
<img src="assets/img/10.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

**Screen**
- Video Memory
    - I set it to maximum, but you need to determine the graphic memory resources you wish to allocate.
- Monitor Count
    - I have dual displays, but only utilize 1 for my virtual machine.  Set this accordingly.
- Scale Factor
    - `no changes`
- Graphics Controller
    - You may consider changing this option.
- Acceleration
    - You could enable 3d acceleration.

Remote Display
- `no changes`

Recording
- `no changes`

<br />
<p align="center">
<img src="assets/img/11.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

## Storage

- Controller IDE

- Controller SATA

- Attributes

<br />
<p align="center">
<img src="assets/img/12.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

**Controller IDE**

- Empty Disc
    - Click the empty disc icon to highlight the item as seen below.

<br />
<p align="center">
<img src="assets/img/13.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

- Attributes
    - Select the disc icon to insert the ISO image you downloaded from [Iso Download].
        - Use the drop down menu to navigate to the location where you saved the ISO image.

<br />
<p align="center">
<img src="assets/img/14.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />

You should observe the ISO image populated into the **Controller IDE** now.

<br />
<p align="center">
<img src="assets/img/15.png" alt="linux" width="600" height="300"/> </a>&nbsp; &nbsp; 
</p>
<br />


---

[Oracle]: https://www.oracle.com/linux/
[ISO Download]: https://yum.oracle.com/oracle-linux-isos.html
[Virtualbox Download]: https://www.virtualbox.org/wiki/Downloads
[email]: attacktheosi@gmail.com

