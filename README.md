# GL-MiFi-SS

GL.iNet GL-MiFi 4G Smart Router
install shadowsocks v3.3.5 on official firmware Version: 3.203


Official website
https://www.gl-inet.com/products/gl-mifi/

OpenWrt
https://openwrt.org/toh/gl.inet/gl-mifi



Compile with OpenWrt SDK


compile shadowsocks

Download OpenWrt SDK
https://downloads.openwrt.org/releases/19.07.7/targets/ath79/nand/openwrt-sdk-19.07.7-ath79-nand_gcc-7.5.0_musl.Linux-x86_64.tar.xz

Download OpenWrt Shadowsocks-libev source code (v3.3.5)
https://github.com/shadowsocks/openwrt-shadowsocks

move the folder to package

make menuconfig

in network select shadowsocks then exit

make package/shadowsocks-libev/compile V=99

compiled ipk file will under bin/package/


compile sample obfs

Download sample obfs source code 
https://codeload.github.com/aa65535/openwrt-simple-obfs/

move the folder to package

make menuconfig

in network select obfs then exit

make package/sample-obfs/compile V=99

compiled ipk file will under bin/package/
