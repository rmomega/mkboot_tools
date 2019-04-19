mkbootimg_tools
===============

### Unpack and repack boot.img,support dtb(dt.img):
./mkboot t.img t
Unpack & decompress t.img to t
  kernel         : /home/ubuntu/ray/mk/t/zImage
  ramdisk        : /home/ubuntu/ray/mk/t/ramdisk.gz
  page_size      : 2048
  base_addr      : 0x80000000
  kernel size    : 6592232
  kernel_addr    : 0x80008000
  ramdisk_size   : 5230616
  ramdisk_addr   : 0x84000000
  second_size    : 0
  second_addr    : 0x80f00000
  cmdline        : bootopt=64S3,32S1,32S1
Unpack completed.




./mkboot t tt.img
mkbootimg from t/img_info.
  kernel         : /home/ubuntu/ray/mk/t/zImage
  ramdisk        : /home/ubuntu/ray/mk/t/new_ramdisk.gz
  page_size      : 2048
  base_addr      : 0x80000000
  kernel size    : 6592232
  kernel_addr    : 0x80008000
  ramdisk_size   : 5230616
  ramdisk_addr   : 0x84000000
  cmdline        : bootopt=64S3,32S1,32S1
Kernel size: 6592232, new ramdisk size: 5242383, tt.img: 11837440.
tt.img has been created.

		...

		xiaolu@xiaolu-ubuntu64:~/e330s$ mkboot t.img t/ramdisk tt.img
		Repack t.img & ramdisk t/ramdisk to tt.img
		  kernel         : /tmp/mkboot.fAJL/zImage
		  ramdisk        : /tmp/mkboot.fAJL/ramdisk.gz
		  page_size      : 2048
		  base_addr      : 0x00000000
		  kernel size    : 6911360
		  kernel_addr    : 0x00008000
		  ramdisk_size   : 2685222
		  ramdisk_addr   : 0x02000000
		  second_size    : 0
		  second_addr    : 0x00f00000
		  dtb_size       : 1427456
		  dtb_img        : /tmp/mkboot.fAJL/dt.img
		  tags_addr      : 0x01e00000
		  cmdline        : console=null androidboot.hardware=qcom user_debug=31 maxcpus=2 msm_rtb.filter=0x3F
		Kernel size: 6911360, new ramdisk size: 3426207, recovery.img: 11767808.
		recovery.img has been created.
		...
