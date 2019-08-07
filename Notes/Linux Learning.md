## Linux Learning

A learning note of Kali Linux

###### Created by Weber Huang



#### 1. Download

#### 2. Setup

#### 3. Linux  



###  Download

___

* [Download Kali Linux from here](https://www.kali.org/downloads/)

* [Download Virtual Box from here](https://www.virtualbox.org/)

After setting up **Virtual Box**,  open the it and choose start to install Kali Linux.

Some of the important step

### Setup

___





### Linux

___

Now we can sign in the Kali Linux as root admin. Make sure keep this password saved. You also can add more sub-account if it isn't necessary to log in with root every time.

**Q1**. One of the problem is that the **Kali's UI** seems to be sub-screen but we want a full-windows screen version. What should we do?

**A1**. Install **VirtualBox guest additions**

(1) Select `Devices` -> `Insert Guest Additions CD image`. If the `VirtualBox`prompts:

```
Unable to insert the virtual optical disk C:\Program Files\Oracle\VirtualBox\VBoxGuestAdditions.iso into the machine CentOS.

Would you like to try to force insertion of this disk?

Count not mount the media/drive 'C:\Program Files\Oracle\VirtualBox\VBoxGuestAdditions.iso' (VERR_PDM_MEDIA_LOCKED).
```

It means the `Devices` -> `CD/DVD DEvices` already has `ISO` file. Please inject it, and try `Insert Guest Additions CD image` again.

(2) Mount the `ISO` file:

```
mount /dev/cdrom /mnt
```

(3) Install the `VirtualBox` guest additions (Take `Linux` as an example):

```
cd /mnt
./VBoxLinuxAdditions.run
```



