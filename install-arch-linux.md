# Steps to Install Arch Linux in VirtualBox on Windows 11

### Download the Arch Linux.
Once done, you need to head to Arch Linux’s official website to download the ISO file. [Click here](https://archlinux.org/download/)

![image](https://user-images.githubusercontent.com/100128996/182668840-573f0367-3bb9-4e8b-93ee-a7fb41e507dd.png)

### Creating the Virtual Machine.
Launch VirtualBox and click on “New” to create a virtual machine.

![image](https://user-images.githubusercontent.com/100128996/182669192-67d87c73-3a01-4d79-8d64-6f914750db55.png)

Enter the name of your virtual machine, it should auto-detect the “Type” and “Version” respectively when you type in “Arch Linux” in the name field.

![image](https://user-images.githubusercontent.com/100128996/182669518-93f090b4-bb76-47bc-aec9-126536f001f4.png)

You should increase the memory size to use the virtual machine comfortably. If it is just for minor testing, you can go ahead with the default setting.
In my case, I allocate ~4 GB of RAM.

![image](https://user-images.githubusercontent.com/100128996/182669784-dc5a5f28-880e-4060-9381-b2dd42574b0b.png)

Also, make sure to create a virtual hard disk under the “Hard disk” option. It should be the selected option by default.

![image](https://user-images.githubusercontent.com/100128996/182669885-d260673f-2485-4a14-92d8-d63e3cc3f414.png)

Next, you need to select the hard disk file type as “VDI (VirtualBox Disk Image)” and the storage as “Dynamically allocated,” as shown in the image above.

![image](https://user-images.githubusercontent.com/100128996/182670227-b5167448-1590-43c6-9eec-1d03f7c130c7.png)

![image](https://user-images.githubusercontent.com/100128996/182670252-8a3f3db5-4362-4508-8b8a-43156c210197.png)

You can choose a preferred location path for the virtual hard disk and tweak the size as per your requirements. The installation should not be a problem with the minimum allocated size (8 GB), but to be on the safe side, you may want to allocate at least 10-15 GB.

![image](https://user-images.githubusercontent.com/100128996/182670424-5f8edbee-a90e-4132-b095-52aee9c0ae96.png)

### Adding the ISO File to Start Installing Arch Linux

![image](https://user-images.githubusercontent.com/100128996/182671422-0e3782a3-b5b7-49ee-8e62-39827137e7e3.png)

![image](https://user-images.githubusercontent.com/100128996/182671668-ed05e1b2-03c8-433a-862e-3d8e96d850a5.png)

Once you select it, hit “OK” to save the changes to your setting.

Now, hit “Start” to start the VM and get started with the installation.

![image](https://user-images.githubusercontent.com/100128996/182672000-fb3fa995-01f7-467f-9575-601ce2bb28cb.png)

Moving on to the installation, when you start the VM, you will be looking at this screen:
The first option is the ideal way of proceeding. If you have a specific requirement, you can choose other options to boot up Arch Linux.

![image](https://user-images.githubusercontent.com/100128996/182805377-f920e502-2a55-414a-ab43-4d07230fad54.png)

Type in “archinstall” to initiate installation using the guided installer.

![image](https://user-images.githubusercontent.com/100128996/182806154-d577c05e-d471-4c57-902d-32edf8bd6bb2.png)

You can choose a keyboard , Timezone , region , in this setting.

![image](https://user-images.githubusercontent.com/100128996/182806514-de990bc9-9ece-4350-bcda-b8d37a9039ea.png)

Select disk layout.

![image](https://user-images.githubusercontent.com/100128996/182809818-b3a5b9a0-094a-48b6-9a96-8f3c27136144.png)

Select Wipe all selected drives and ... " Enter "

![image](https://user-images.githubusercontent.com/100128996/182809884-15e60b30-3fb0-46b3-8123-b39fed915592.png)

Choose btrfs and "Enter"

![image](https://user-images.githubusercontent.com/100128996/182809985-46f19448-4145-42b4-8e76-74ea91d31b88.png)

Choose yes(default)

![image](https://user-images.githubusercontent.com/100128996/182810102-1f027b33-82c0-4b91-80b2-1c89a1f262d8.png)

Set your root password.when you complete setting go to install.

![image](https://user-images.githubusercontent.com/100128996/182810522-99dd6e28-7158-47ad-9a5e-38f8df37c7f0.png)

"Press Enter"

![image](https://user-images.githubusercontent.com/100128996/182810607-05ba6454-40ad-4c44-a388-b7e83021f853.png)

It will take a few minute to install .

![image](https://user-images.githubusercontent.com/100128996/182810902-e5b47762-e79e-4d60-8c0f-4798654f5e42.png)

Choose " Yes "

![image](https://user-images.githubusercontent.com/100128996/182812551-9d678a52-b424-48e3-9322-5b31e9439cb4.png)

Your install almost complete now you need to reboot virtualbox.
After you reboot your virtualbox and open it click setting and go to storage .

![image](https://user-images.githubusercontent.com/100128996/182813407-8a74b299-f2cf-439c-8654-c24bc5717cdb.png)

![image](https://user-images.githubusercontent.com/100128996/182813593-b01a1c81-4537-48e5-a798-ba04641ba64c.png)

Right click the iso file and remove it .

![image](https://user-images.githubusercontent.com/100128996/182813915-bed2b05a-ae78-4dcb-a536-5b5e11f85bde.png)




