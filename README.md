#Ubuntu Extending HDD Space

1) Boot into "Try Ubuntu" mode with iso image
2) Use gParted to extend the drive
3) boot back into the main ubuntu drive

Commands to Extend (Use sudo or root):
1) vgdisplay
2) lvdisplay
3) lvextend -l +100%FREE /dev/ubuntu-vg/ubuntu-lv
4) lvdisplay
5) df -h
6) resize2fs /dev/mapper/ubuntu--vg-ubuntu--lv
7) df -h

Resources:
https://packetpushers.net/ubuntu-extend-your-default-lvm-space/
