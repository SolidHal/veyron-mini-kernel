# Minimized kernel for the c201


Linux libre kernel for the asus c201 (veyron_speedy) minimized
experimenting for linuxboot
Drops support for many drivers, and all networking that would be useless in a bootloader environment. 


Size comparison:
Before:
```
root@PrawnOS-Desktop-Builder:~/PrawnOS/build/linux-5.4.23/arch/arm/boot# ls -lah
-rwxr-xr-x   1 root root  23M Jan 19 01:05 Image
-rwxr-xr-x   1 root root  12M Jan 19 01:05 zImage

```

After:
```
root@PrawnOS-Desktop-Builder:~/veyron-mini-kernel/build/linux-5.4.23/arch/arm/boot# ls -lah
-rwxr-xr-x  1 root root 9.3M Mar 20 18:02 Image
-rwxr-xr-x  1 root root 3.1M Mar 20 18:02 zImage
```

likely can get smaller by dropping prink support
