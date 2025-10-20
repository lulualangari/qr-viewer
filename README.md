# 🌿 Ardara QR Motivation Project  

A simple web project developed by Ardara’s Digital & Innovation Team.  
The system generates one QR code that displays a **new motivational quote** every time it’s scanned — designed to inspire creativity and positivity among team members.  

---

## 💡 Project Idea  
- One QR code available to everyone.  
- Each scan retrieves a **different quote** from a Firebase Realtime Database.  
- Every quote appears only once per cycle (no repetition).  
- Built using HTML, CSS, and Firebase — no backend required.  
- Designed with Ardara’s official colors and logo.  

---

 🛠️ Technologies Used  
- **HTML / CSS / JavaScript**  
- **Firebase Realtime Database**  
- **GitHub Pages** for hosting  
- **QR Code** generated via [QRCode Monkey](https://www.qrcode-monkey.com)

---

## ⚙️ How It Works  
1. Each scan (or page load) increments a counter `nextSeq`.  
2. The system fetches the next available quote from Firebase under `/messages/{number}`.  
3. Once displayed, that quote is marked as `used: true`.  
4. When all quotes are used, the admin can reset the cycle manually.  

---

