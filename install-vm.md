# Steps to Install Ubuntu linux in VirtualBox on Windows 11

![ubuntuGif](images/Ubuntu_gif.gif)

### YOUR PC REQUIRED SPEC !
You will need : [required processor, memory, and hard drive space](https://www.virtualbox.org/wiki/End-user_documentation)

### Download the Ubuntu.
Check Ubuntu Releases to find the latest version of Ubuntu that has long term support (LTS).the latest release is Ubuntu 22.04 LTS. You can download another version if you want . [link download](https://ubuntu.com/download/desktop) and when your download complete you will get .iso file. 

![image](https://user-images.githubusercontent.com/100128996/182571580-d308b973-498b-46d9-a6cd-03b629ebef69.png)

### Install VirtualBox.
You can watch this video to install Virtualbox  [go to video](https://www.youtube.com/watch?v=b866-7Y_0KQ)
  
  ![image](https://user-images.githubusercontent.com/100128996/182576705-084aec64-ff56-4080-8c6f-596c7c00e450.png) 
  
### Create a Virtual Machine.
**Now that VirtualBox is installed on your computer, we need to now create a new virtual machine.
Click the New button in the toolbar.**

![image](https://user-images.githubusercontent.com/100128996/182580219-5cea5e59-11fa-46d4-b549-bc5be926bf9c.png)

Type in a descriptive name for your operating system. You can stick with the default machine folder. The machine folder is where your virtual machines will be stored.

![image](https://user-images.githubusercontent.com/100128996/182580574-327b5a9a-88e4-4814-b22c-bb3154987a49.png)

choose the memory size you want to give a virsual machine.If you think it not enough ,You can comeback and change agian later .

![image](https://user-images.githubusercontent.com/100128996/182581047-78fead17-a086-4abe-8b7f-aba93a2a1edc.png)

Make sure “Create a virtual hard disk now” is selected, and click Create.

![image](https://user-images.githubusercontent.com/100128996/182582111-765f5442-cdb4-4eea-9a37-6c2e1f6a736f.png)

Select “VirtualBox Disk Image (VDI)”, and click Next.
Choose a Fixed size virtual hard disk so that you have better performance, and click next.

![image](https://user-images.githubusercontent.com/100128996/182582838-760ab49e-3e30-4294-a61f-3d0eedeb34df.png)

choose hard disk space for Virtual box.

![image](https://user-images.githubusercontent.com/100128996/182583125-43bcc550-dc82-4425-9d22-3e1d7b5f88d0.png)

Double-click on the left panel where it says “Ubuntu 18.04.” A startup window will appear.

![image](https://user-images.githubusercontent.com/100128996/182583746-f0903f07-ff20-452c-8fb9-b81a56a473ab.png)

Click the Folder icon next to Empty and select the Ubuntu image you downloaded earlier in this tutorial. It is a .iso file. You can make sure that your .iso file is somewhere in your C drive (doesn’t have to be on your Desktop). Then click Start to proceed.

![image](https://user-images.githubusercontent.com/100128996/182597175-5fea75fa-e4c4-4dd3-9084-bb383a3d6ed0.png)

You might get an error that looks like this.

![image](https://user-images.githubusercontent.com/100128996/182603151-cf9319c7-d18d-4f16-8d56-a1f045f81608.png)

Click Close VM.

### Enable Virtualization Technology on Your Computer.
The error above arises because virtualization technology is disabled on your computer by default. We need to enable it. Let’s do that now.
[Click here](https://www.youtube.com/watch?v=UMo-is3fjPI)

when you complete Enable Virtualization and reboot your computer.
Double-click on the VirtualBox icon to start it.
Click on the left panel of the window to start the Ubuntu virtual machine. Or you can just click Start in the toolbar.

![image](https://user-images.githubusercontent.com/100128996/182602875-80f50355-9d29-4598-a1f2-67beef6f4035.png)

### Install Ubuntu
Click on “Install Ubuntu” to install Ubuntu.

![image](https://user-images.githubusercontent.com/100128996/182602685-669ddc97-4b95-4ac0-92ef-0a1692c4cfad.png)

Click “Continue” to save the keyboard layout. The default English one is fine.

Keep clicking Continue through all the prompts. The options you want selected as you go through the prompts are the following:

* Download updates while installing Ubuntu
* Erase disk and install Ubuntu

You will get to a point where you will need to set your time zone. It will be a big map of the world that should automatically detect your location.
Type in a computer name and pick a username and password. I select the “Log in automatically” option.

When installation is complete, click “Restart Now.”












