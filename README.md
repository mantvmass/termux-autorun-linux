# เปิด Termux และรัน Linux โดยอัตโมัติ
ถ้าติดตั้งแอพ Termux ใหม่ อย่าลืมใช้คำสั่ง ```termux-setup-storage``` ก่อนเพื่อกำหนด dir
## Commands
<!-- [ ให้ติดตั้ง Linux(Ubuntu) เมนูที่ 1 ผ่าน os-installer ให้เรียบร้อยก่อน ](https://github.com/mantvmass/os-installer) -->

```
pkg install nano && cd /data/data/com.termux/files/usr/etc && nano profile
```

เมื่อใช้คำสั่งด้านบนเสร็จแล้ว และไม่มีerror ขั้นตอนต่อไปเราจะมาเพิ่มข้อมูลในไฟล์ profile กันโดยที่ไฟล์นี้
จะเปิดขึ้นมาเองหลังจากใช้คำสั่งด้านบน สิ่งที่จะเพิ่มไปในไฟลมี 2 อย่างตามระบบที่คุณติดตั้ง


## os-installer เพิ่มข้อมูลนี้ใน profile บรรทัดสุดท้าย
```
cd && cd /data/data/com.termux/files/usr/etc/os-install
sh ubun.sh
```

## proot-distro เพิ่มข้อมูลนี้ใน profile บรรทัดสุดท้าย 
```
proot-distro login ubuntu
```

## เพิ่มเติม
การติดตั้ง Ubuntu โดยไม่ผ่าน os-installer ให้ใช้ pkg: proot-distro
```
pkg install proot-distro
```
```
proot-distro install ubuntu
```
