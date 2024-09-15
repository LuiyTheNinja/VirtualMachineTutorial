<h1>1. Download and install VirtualBox</h1>
<h3>Step 1: Download Virtual Box</h3>
- [Go to the Oracle VirtualBox Website](https://www.virtualbox.org/)
</br>
- Select the appropriate version for your Operating System (Windows, macOS, or Linux)
</br>
- Click the Link to download and follow the installer instructions to complete the installation.

<h3>Step 2: Install VirtualBox Extension Pack(Optional, but Highly Recommended)</h3>
- Download the Extension Pack from the Same VirtualBox download page.
</br>
- After downloading, open VirtualBox;
</br>
GO TO: File > Preferences > Extensions, and click the "+" icon to install the Extension Pack. 
</br>

<h1>2. Set Up Your First Virtual Machine</h1>
<h3>Step 1: Launch VirtualBox</h3>
</br>
- Open VirtualBox and Cleck "New" button to create a new virtual machine. 

<h3>Step 2: Name and Select Operating System</h3>
</br>
- Name your VM (ex, Kali Linux for Penetration Testing).
</br>
- Type: Choose the OS Type (Linux, Windows, etc.)
</br>
- Version: Select the Version of the OS (ex, Ubuntu 64-bit, Windows 10 64-bit, etc).

<h1>3. Resource Allocation Settings</h1>
<h3>Step 1: Allocate Memory</h3>
<br/>
- Allocate at least 2 GB of RAM for Linux Distributions, but 4GB OR higher is recommended for Windows or more resource-intensive tasks. 
<br/>
(NOTE: Ensure that you do not allocate more than 50% of your host nachine's RAM)

<h3>Step 2: Create Virtual Hard Disk</h3>
<br/>
- Choose "Create a virtual hard disk now" and click "Create"
<br/>
- Select the hard disk file type as VDI(Virtual Disk Image)
<br/>
- Select "Dynamically Allocated" For efficient use of space
</br>
(This allows the virtual hard disk to grow as needed)
<br/>
- Allocate at least 20 GB of disk space for Linux and 30 GB or more for Windows

<h1>4. Configure Virtual Machine Settings</h1>
<h3>Step 1: CPU Allocation</h3>
<br/>
- In the "System" tab, go to the "Processor" Tab.
      - Allocate 2 CPU cores for general use. For advanced use or heavy software. 
</br>
      (Like cybersecurity tools or penetration test, in which you should allocate 4 cores if your machine supports it.)
<br/>
<h3>Step 2: Configure Display</h3>
<br/>
- In the "Display" tab, increase video memory to at least 128 MB for smooth performance
<br/>
(ESPECIALLY Important for Graphical User interface(GUI)-based Operating Systems))

<h1>5. Download Operating System ISO Files</h1>
<h3>Step 1: Get the ISO</h3>
<br/>
- For Linux OS(Ubuntu, Kali, Parrot, etc), download the ISO from the official website:
    - [Kali Linux](https://www.kali.org/get-kali/#kali-virtual-machines)
          -(NOTE: Do not use the Pre-built Virtual Machines for this tutorial, use "Installer Images")
    - [Ubuntu](https://ubuntu.com/download)
    - [ParrotOS](https://parrotsec.org/download/)
<br/>
- For Windows OS, you can download ISO files from the [Microsoft Website](https://www.microsoft.com/en-us/software-download/).

<h1>6. Install the Operating System</h1>
<br/>
<h3>Step 1: Attach the ISO File</h3>
<br/>
- After Downloading the ISO file, Go to your Virtual Machine Settings. 
<br/>
- In the "Storage" section, click on the empty CD icon, then click the small CD icon on the right-hand side. 
<br/>
- Choose "Choose a disk file...", and select the ISO file you downloaded.

<h3>Step 2: Start The Virtual Machine</h3>
<br/>
- Go back to the main VirtualBox window, select the VM, and click Start.
- Follow the prompts to install the Operating System on the virtual Machine. 

<h1>7. Post-Installation Configuration</h1>
<br/>
<h3>Step 1: Install Guest Additions(Option but Recommended)</h3>
<br/>
- Once the OS is installed, you can improve performance and usability by installing VirtualBox Guest Additions. 
<br/>
- In the running VM, go to Devices > Insert Guest Additions CD Image and follow the prompts to install. 
<br/>
This step will enhance screen resolution, clipboard sharing, and drag and drop between host and guest OS. 
<br/>

<h1>8. Networking Settings for Cybersecurity Labs</h1>
<br/>
<h3>Step 1: Configuring Network for Pentesting Labs</h3>
<br/>
- Go to the "Network" tab of your VM Settings. 
<br/>
- Select "Bridged Adapter" for real network interaction, which allows the VM to behave as if it's connected to your local network,
<br/>
useful for pentesting labs. 
<br/>
- For isolated testing, Choose "NAT" or "Internal Network" to create a safe, enclosed environment.
<br/>

<h1>9. Creating and Cloning VM's for Lab Environments</h1>
<br/>
<h3>Step 1: Save a Baseline Image</h3>
<br/>
- Once you've installed your Operating System and necessary software, you can create a "snapshot" in VirtualBox to save the state of your virtual machine.
<br/>
- Go to Machine > Take Snapshot to save the Virtual Machine State.
<br/>
<h3>Step 2: Clone a Virtual Machine</h3>
<br/>
- If you want to create identitcal VM's, with the same settings, you can clone the VM. 
<br/>
- Right-click on your VM in the main menu, select "Clone", and follow the prompts to create an identitcal copy.
<br/>

<h1>10. Suggested Settings for Cybersecurity VM's</h1>
<br/>
Here are some suggested resource allocations for common Operating Systems used in cybersecurity labs:
<br/>
<br/>
Kali:
<br/>
<br/>
      - RAM: 4 GB
<br/>
      - CPU: 2-4 Cores
<br/>
      - Disk: 25 GB
<br/>
<br/>

Parrot OS: 
<br/>
<br/>
      - RAM: 2-4 GB
<br/>
      - CPU: 2 Cores
<br/>
      - Disk: 20 GB
<br/>
<br/>
Windows 11:
<br/>
<br/>
      - RAM: 4-8 GB
<br/>
      - CPU: 4 Cores
<br/>
      - Disk: 30-40 GB
<br/>

<h1>11. Security Considerations</h1>
<br/>
<h3>Step 1: Isolate Your Lab</h3>
<br/>
- For any cybersecurity testing, it's good practice to isolate your VM's from the hose machine or external network.
<br/>
(Use Intermal Network mod for added Safety)
<br/>
<h3>Step 2: Take Regular Snapshots</h3>
<br/>
- Before running any experiments or pentesting tasks, always take snapshots of the current state of your VM, so you can roll back if something goes wrong. 
<br/>

<h1>12. Final Notes</h1>
<br/>
By following this guide, you can effectively set up virtual machines for cybersecurity labs. With proper configuration of resources, networking, and isolations, you'll have a flexible environment to test tools, practice penetration testing, and devlop skills for cybersecurity scenarios. 
