# Student Info App (React Native + Expo)

แอปข้อมูลนักศึกษา 2 หน้า (Main Page และ Registration Page) พัฒนาโดยใช้ React Native Paper (MD3) และ React Navigation ภายใต้ Expo

## เทคโนโลยีที่ใช้
- Expo SDK: 50.x.x
- React Native: 0.73.x
- React Native Paper: 5.x.x
- React Navigation: 6.x.x
- react-native-safe-area-context
- react-native-screens

## วิธีติดตั้งและรัน

1. **เปิดโครงการใน VS Code**
   โครงงานนี้สร้างจาก template `expo blank`  
   ```bash
   npx create-expo-app student-info-rn --template blank

2. **ติดตั้งไลบรารีที่ใช้**
npm install @react-navigation/native @react-navigation/native-stack
npm install react-native-paper
npm install react-native-safe-area-context react-native-screens

3. **รันแอป**
npx expo start

4. **ทดสอบบน Android**
หากใช้ Android Emulator → เปิด Android Studio, รัน Emulator จากนั้นเลือก Run on Android emulator ใน Expo

**หน้าจอในแอป**
1. Man Page
- แสดงข้อมูลนักศึกษา: ชื่อ, นามสกุล, รหัสนักศึกษา, สาขา, สำนักวิชา
- แสดงรูปจาก URL ด้วย Avatar.Image
- ปุ่มนำทางไปหน้า Registration Page
2. Registration Page
- แสดงรายวิชาแยกตามเทอมด้วย List.Accordion
- แสดงรายวิชาในรูปแบบ รหัส – ชื่อวิชา
