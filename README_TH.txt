Car Media v1.5
โครงสร้าง: S25 -> UDP 8766 -> PC -> TROFEO USB
- ใช้ UDP ที่ v1.4.1 พิสูจน์แล้วว่าถึง PC
- PC Bridge ส่ง JPEG ล่าสุดเข้า TROFEO
- Latest Frame: ถ้า USB ช้าจะทิ้งภาพเก่า
- Android 960x360, JPEG Q30, จำกัดประมาณ 20 FPS

วิธีทดสอบ
1. ปิด TRCC และ InfoPanel
2. Firewall UDP 8766 เปิดไว้แล้วจากการทดสอบก่อนหน้า
3. ปิด Diagnostic v1.4.1 ก่อน (สำคัญ เพราะใช้ port 8766 เดียวกัน)
4. เปิด PC_Bridge/START_CAR_MEDIA_v1_5.bat
5. ติดตั้ง/เปิด Car Media v1.5
6. START SCREEN MIRROR > Entire screen
7. Bridge ควรขึ้น TROFEO READY และค่า RX / USB เพิ่มขึ้น
8. ทดสอบ YouTube แล้วดู latency
