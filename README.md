the story was started by 20 s905L-B tv box that I gought from china 
this is about s905L-B s905L-2 S905M-B S905M-2
17/04/2019 update =====================================================================================================================

# gxl-s905L-B-p211
unpacke from p211 dtb

the firmware I unpacked from: https://drive.google.com/file/d/1PaGA-DdopQlabnQ3tYAcCukSB_Ui1G83/view?usp=sharing
https://forum.xda-developers.com/devdb/project/dl/?id=31240 tool for unpacking 


13/02/2020 update =====================================================================================================================

I found linux kernel added s905m2 to it https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/tree/drivers/soc/amlogic/meson-gx-socinfo.c?h=v5.4.19 then I saw someone got a s905m2 device with P211 (but s905m2 shloud boot with P212 DTB right?) setup on chinese forum so I started to find the way to install armbian(a linux optreating system???) on it .in the end it was end up with a armbian on sd card and booted to the armbian with p212 dtb so I guess most of android 8.0 for s905x can also work with p211 devices but aml flash tool just won't let us flash it in

========================================================================================================================================
so the way to make P211 devices to boot from sd card(I TRIED USB AND IT WON'T WORK!!!) is downlaod this image for P211 with TWRP recovery and SUPERSU :https://drive.google.com/file/d/14d4OiMTjTe-zmTQZcKm_aaH5Xh28ZgHN/view?usp=sharing then flash it in to the tv box by using amlogic burning tool install android terminal emulator to the tv box type :su to make sure android terminal emulator get root access

then type :reboot update 

=========================================================================================================================================
https://drive.google.com/file/d/1wuZNPSorJEmi19ZFN_qbXblUOtdSxVwi/view?usp=sharing for armbian image( do remember to change dtb file to p212)
then u shloud burn this image to sd card 
login
account :root
password: 1234

hope this helps you 
