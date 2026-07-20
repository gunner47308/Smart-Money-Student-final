# Smart Money Student

Progressive Web App (PWA) สำหรับนักศึกษา เพื่อบันทึกรายรับรายจ่ายแบบออฟไลน์ พร้อมการจัดหมวดหมู่จากข้อความธรรมชาติ

## Features

- บันทึกรายรับและรายจ่ายด้วย Local Storage
- วิเคราะห์ข้อความ เช่น `ข้าว 50` หรือ `Grab 120` เพื่อระบุจำนวนเงินและหมวดหมู่
- Dashboard สรุปยอด รายรับ รายจ่าย กราฟหมวดหมู่ และแนวโน้มค่าใช้จ่าย 7 วัน
- ตั้งงบประมาณรายเดือน พร้อมแจ้งเตือนเมื่อใช้งบเกิน
- เปลี่ยนภาษาไทย / English จากหน้าโปรไฟล์
- ส่งออกและนำเข้าข้อมูล JSON
- PWA พร้อม manifest และ service worker
- ใช้งานได้โดยไม่ต้องมี backend

## Run locally

เปิดไฟล์ `index.html` ในเบราว์เซอร์ได้ทันที

สำหรับการติดตั้งเป็น PWA และให้ Service Worker ทำงานครบถ้วน แนะนำให้รันผ่าน local server เช่น VS Code Live Server หรือ:

```bash
python -m http.server 8080
```

จากนั้นเปิด `http://localhost:8080`

## Project structure

```
smart-money-student/
├── assets/          # Logo and app assets
├── css/             # Responsive styling
├── js/              # Authentication, storage, parser, charts, UI
├── index.html       # Splash screen
├── dashboard.html   # Main dashboard
├── manifest.json
└── service-worker.js
```

## Data privacy

ข้อมูลทั้งหมดจัดเก็บเฉพาะในเบราว์เซอร์ของผู้ใช้ด้วย Local Storage ไม่มีการส่งข้อมูลไปยังเซิร์ฟเวอร์ภายนอก

## License

MIT License — see [LICENSE](LICENSE).
