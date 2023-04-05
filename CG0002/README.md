# Create a shared folder between virtual os and host os

<https://youtu.be/GixtTVx_eGc>

## Enable vsboxsf

- start virtual os (Ubuntu)

<img src="cg0002a.png" alt="VM1" width="600"/>

- open terminal
- cd /media
- cd codersgossips (your user name)
- cd VBox_GAs_7.0.6
- sudo ./VBoxLinuxAdditions.run

<img src="cg0002b.png" alt="VM1" width="600"/>

## Create a shared folder

- Click on Devices
- Shared Folders
- Shared Folder Setting

<img src="cg0002c.png" alt="VM1" width="600"/>

- Choose your windows folder
- Enter a folder name
- check **Auto-mount**
- check **Make-Permanent**

<img src="cg0002d.png" alt="VM1" width="600"/>

## Link folder

- cd ~
- sudo mkdir win_shared
- sudo mount -t vboxsf win_shared ~/win_shared
  - here **win_shared** is same folder name which you given in folder settings.
