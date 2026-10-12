# Gold Trading Dashboard — รุ่นแก้ไขปัญหาโหลดราคา

รุ่นนี้เปลี่ยนจากการเรียก `fetch()` ไปที่ GoldPrice.dev API โดยตรง มาใช้ GoldPrice.dev Official Widget ผ่าน `iframe` เพื่อหลีกเลี่ยงปัญหา browser CORS และไม่ต้องใช้ API key ในหน้าเว็บ

## เผยแพร่ผ่าน GitHub Pages

1. ดาวน์โหลด ZIP และแตกไฟล์
2. เปิด GitHub repository เดิมที่ใช้เผยแพร่ `gold-trading-dashboard`
3. เลือก **Add file → Upload files**
4. อัปโหลด `index.html` จากโฟลเดอร์นี้ทับไฟล์เดิมที่ root ของ repository
5. กด **Commit changes** แล้วรอ GitHub Pages เผยแพร่การแก้ไข
6. เปิด URL GitHub Pages ใหม่ กดรีเฟรชแบบ hard refresh หากเห็นเวอร์ชันเก่า
7. หากใช้ Notion Embed ให้รีเฟรชหรือเปิด URL เดิมใหม่หลังเว็บไซต์อัปเดต

## การแสดงราคา

- ใช้ iframe: `https://goldprice.dev/embed/xau?currency=USD&unit=oz&karat=24&theme=dark&locale=en`
- Widget จะอัปเดตตัวเองประมาณทุก 60 วินาที
- ไม่มี API key ในไฟล์
- ต้องคง attribution/ลิงก์ “Powered by goldprice.dev” ที่ widget ให้มาไว้ตามข้อกำหนดของผู้ให้บริการ
- ราคา Spot reference ไม่ใช่ Bid/Ask ของ HUA SENG HENG หรือ MTS Gold

## หากยังไม่แสดงราคา

1. เปิด URL iframe โดยตรงในเบราว์เซอร์: `https://goldprice.dev/embed/xau?currency=USD&unit=oz&karat=24&theme=dark&locale=en`
2. หาก URL นี้เปิดไม่ได้ อาจเป็นปัญหาเครือข่ายหรือผู้ให้บริการ widget
3. หาก iframe เปิดได้โดยตรง แต่ไม่แสดงใน GitHub Pages ให้ตรวจ URL เว็บไซต์ที่เผยแพร่และ Browser Console
4. หาก GitHub Pages แสดงได้ แต่ใน Notion ไม่แสดง ให้ตรวจว่า Notion อนุญาต Embed ของ URL นั้นหรือไม่
