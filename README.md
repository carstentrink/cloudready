Steps to disable rootfs verification:

1) Log in

2) Press ```ctl+alt+t``` to open a terminal

3) Type in ```shell``` and hit enter

4) Confirm that the yellow ```crosh``` prompt is now a green ```chronos@localhost``` prompt

5) Disable rootfs verification:

```sudo disable_verity```

6) Reboot your device:

```sudo reboot```

7) Now you can log in and proceed with rootfs edits as you normally would. You will still need to remount root as read/write:

```sudo mount -o rw,remount /```


Home-Edition Users:

For home edition users and users whose machines are un-managed you can halt the updates via command line or by blocking the following urls in your filtering device/firewall :

Update Server: cloudready-paid-update-server-2.neverware.com 

Update Storage URLs: cloudready-paid-update-storage.neverware.com

Legacy Update Server: cloudready-update-server-2015-03-12.neverware.com

Home Edition Update Server: cloudready-free-update-server-2.neverware.com
