## Installing Windows on VirtualBox on Ubuntu 

* Install VirtualBox for Ubuntu with `sudo apt-get install virtualbox`
* Get Windows 10 ISO
* Open VirtualBox and create a new VM. Select RAM and File Location and Disk Size.
* Setting -> Storage add the ISO file and Disk Storage Created
* Click Start Icon and Windows will start installation. 
* After installatin is done, Click on Devices -> Insert Guest Additions CD Images. It will start downloading. After Completing Download CD image will be
visible Under windows file manager. Click and install it. It is needed for using full window feature, file sharing and some other
options. 

* For Sharing folder from host os:

**On Host OS:**

* To add Folder:

`vboxmanage sharedfolder add "VMName" --name "SharedFolderName" --hostpath "SharedFolderPathOnHost"`

* To remove a Shared folder:

`vboxmanage sharedfolder remove "VMName" --name "SharedFolderName"`

**On Guest OS:**

* Go to Devices -> Shared Folder -> Shared Folder Settings. Add the shared folder path on the Host os and the name of the folder.

* From windows cmd:

`net use x: \\vboxsvr\"SharedFolderName"`

Now Go to Network bellow This PC on windows. You will find the VBOXSVR and shared folders inside.


