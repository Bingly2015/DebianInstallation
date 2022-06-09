# DebianInstallation(describe the installation of debian) <br>
1.backup the important files in the old version und bookmark history in the explorer
   - pay attention to home, downloads und documents directory. export all the bookmark from the explorer(firefox, i use).
   - in firefox(bookmark-> manage bookmark)<br>
2. Downloads the Debian Version
    - check the internet connection.
    - if yes the netisnt version.
    - varify the check sum of the downloaded file.<br>
3. building a bootable USB containing Debian(11) ISO
    - find out the name the usb in your debian system with lsblk
    - unmount the device with sudo umount /dev/sdb(the name may change)
    - wirte the file to the usb with "sudo dd bs=4M if=/home/bing/Downloads/debian-11.3.0-amd64-netinst.iso of=/dev/sdb status=progress oflag=sync"<br>
        ps: dd is used to convert and copy files including clone disk or wipe data
4. wlan driver
   lspci(Network controller: Broadcom Limited BCM43142 802.11b/g/n (rev 01))<br>
5. language setting(optional)
