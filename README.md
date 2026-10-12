# Gold Trading Dashboard — GitHub Pages


1. เข้าสู่ระบบ GitHub ที่ https://github.com/new
2. สร้าง repository ใหม่ ชื่อ `gold-trading-dashboard` และเลือก **Public** (GitHub Free ต้องใช้ public repository สำหรับ GitHub Pages)
3. กด **Create repository**
4. ใน repository กด **Add file → Upload files**
5. เลือกไฟล์ `index.html` จากชุดนี้ อัปโหลดให้ไฟล์อยู่ที่ root ของ repository (อย่าใส่ไว้ในโฟลเดอร์ย่อย)
6. กด **Commit changes**
7. เปิดแท็บ **Settings → Pages**
8. ในส่วน **Build and deployment** ตั้ง Source เป็น **Deploy from a branch**
9. เลือก branch `main` และ folder `/(root)` แล้วกด **Save**
10. รอการเผยแพร่ แล้วกลับมาหน้า Pages เพื่อเปิด URL เว็บไซต์ที่ GitHub แจ้ง (มักอยู่ในรูป `https://USERNAME.github.io/gold-trading-dashboard/`)
11. เปิด URL นั้นแยกในแท็บใหม่ ตรวจสอบว่าราคาทองและกราฟโหลดได้ก่อน
12. ใน Notion พิมพ์ `/embed` แล้ววาง URL ที่เผยแพร่แล้ว

## หมายเหตุ
- repository แบบ Public หมายถึงไฟล์ HTML และ source code สามารถดูได้โดยสาธารณะ
- หน้าเว็บใช้ GoldPrice.dev API แบบ anonymous ไม่ได้ฝัง API key ไว้ในไฟล์
- หาก Notion ไม่แสดงหน้าเว็บ ให้เปิด URL GitHub Pages โดยตรงก่อน แล้วลองเปลี่ยน URL หรือใช้ผู้ให้บริการโฮสต์ที่อนุญาตการฝัง iframe
- ราคา API เป็นราคา Spot reference ไม่ใช่ราคา Bid/Ask ของ HUA SENG HENG หรือ MTS Gold
