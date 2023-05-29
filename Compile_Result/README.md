# kernel-for-rt-bubbles

复制此文件到树莓派，并执行以下命令

```shell
sudo cp arch/arm64/boot/dts/broadcom/*.dtb /boot/
sudo cp arch/arm64/boot/dts/overlays/*.dtb* /boot/overlays/
sudo cp arch/arm64/boot/dts/overlays/README /boot/overlays/
sudo mv /boot/$KERNEL.img ../
sudo cp arch/arm64/boot/Image.gz /boot/$KERNEL.img
```

断电重启
```shell
sudo reboot
```
重启后内核版本变为 Linux raspberrypi 5.15.49-rt47-v8