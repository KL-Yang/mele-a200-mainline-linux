# mele-a200-Debian-Stretch

Note: Debian stretch armmp kernel fully support this TV-box (except the Mali), 
it works with sun5i-a10s-olinuxino-micro.dts, only a few minor warning due to the hardware difference.

Here provide the original FEX from android firmware and corresponding dts file,
and example 5.1.y (4.10 to 5.0 does not work well somehow) kernel configuration.
The display on HDMI works fine, kernel command line argument should refer to those sunxi device in Armbian.

# U-BOOT
U-BOOT v2016.11 use A10s-OLinuXino-M_defconfig, everything works, including display over HDMI, but NAND is not supported.
For newer version v2019.04 with NAND support, use configuration file and dts file in this u-boot directory.
When enable MUSB, the boot time seems much longer, may be more than 10s.

http://linux-sunxi.org/Mele_A200
