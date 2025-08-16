# Student Info App — Expo (Android)

แอปข้อมูลนักศึกษา 2 หน้า ใช้ **React Native Paper (MD3)** + **React Navigation** บน **Expo**. ทำงานครบผ่าน VS Code + Android.

---

## Quick Start
```bash
npm install
npx expo start
# กด a เพื่อรันบน Android Emulator หรือสแกน QR ด้วยแอป Expo Go
```

> ต้องมี Android Studio (สำหรับ Emulator) หรือมือถือ Android + แอป Expo Go

---

## 🔧 Dependencies (หลัก)
- @react-navigation/native
- @react-navigation/native-stack
- react-native-paper
- react-native-safe-area-context
- react-native-screens

> โปรเจกต์มาจาก template **expo blank** (ไม่ต้องติดตั้ง expo-cli แบบ global ใช้ `npx` ได้เลย)

---

## โครงสร้างไฟล์ (ย่อ)
```
App.js                 # โค้ดหลัก, สร้าง Stack (Main, Registration)
```
> (ถ้ามีไฟล์เพิ่ม แนะนำจัดเป็นโฟลเดอร์ `src/screens`, `src/data` ตามต้องการ)

---

## 🗂 Data Model (สรุป)
- **Course**: `code`, `name`
- **SemesterRegistration**: `term`, `courses: Course[]`
- **Student**: `firstName`, `lastName`, `studentId`, `major`, `school`, `imageUrl`, `registrations: SemesterRegistration[]`

---

## หน้าจอ
- **Main Page**: รายละเอียดนักศึกษา + รูปจาก URL (Avatar.Image) + ปุ่มไปหน้า Registration
- **Registration Page**: รายวิชาแยกตามเทอม (List.Accordion) แสดงแบบ `รหัส – ชื่อวิชา`

---

## Screenshots (ใส่เองภายหลัง)
```
./assets/screenshot-main.png
./assets/screenshot-registration.png
```
เพิ่มใน README ได้ด้วย:
```md
![Main](./assets/screenshot-main.png)
![Registration](./assets/screenshot-registration.png)
```

---

## ℹNotes
- ต้องต่ออินเทอร์เน็ตเพื่อโหลดรูปนักศึกษาจาก URL
- ถ้า Emulator ไม่ขึ้น ให้เปิด Android Studio > Virtual Device Manager > Start ก่อน

