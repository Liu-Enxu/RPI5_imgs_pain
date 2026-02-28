# RPI5_imgs_pain
PAIN... installing non-official supported operating systems

## Arch
Mostly from this: https://kiljan.org/2023/11/24/arch-linux-arm-on-a-raspberry-pi-5-model-b/

Follow [this](ARCH_INSTALL.txt)

## Debian (native)
### rough instructions

https://www.youtube.com/watch?v=SuGiuAw1kg8

https://www.reddit.com/r/debian/comments/1bf3g3v/debian_12_on_raspberry_pi_5/
```
taspenwall•2y ago

I havn't done debian on a pi 5 yet, but I have built many debian images for the RP to have luks and btrfs. You have to build the image using debootstrap and a chroot with qemu. You could probably to it on a pi, but it's much easier with qemu and a debian machine. For the pi5 they changed the layout of where the kernel and initramfs are stored. The kernel/initramfs in the /boot is just there to look pretty, the real one is in /boot/firmware. When you build the image I would install the kernel package and then copy the kernel and initramfs over to firmware. I like to install my kernel with dpkg. I got lost down a rabbit hole with building kernels for the pi 5 into deb packages. You can grab the overlays/device tree from the Raspberry Pi image.

Why not get a nvme hat for the drive and use PCI for the drive?? Kind of the whole point of having a 5.

You will also get a bunch of replys that say the debian images for the PI are not offically supported and that just run PIos as it's pretty much debian.
```

### official Debian links

https://wiki.debian.org/RaspberryPiImages#Build_your_own_Raspberry_Pi_Debian-based_image

https://raspi.debian.net/

https://salsa.debian.org/raspi-team/image-specs

https://github.com/emojifreak/debian-rpi-image-script

### open source community

https://github.com/lueschem/edi-pi

https://gist.github.com/Algorithm0/d2bd2f69ec863e9fe372888278eb0221

### something else

dietPi: https://www.youtube.com/watch?v=FVkNYSURmxk
