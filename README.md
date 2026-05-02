[00-START-HERE.md](https://github.com/user-attachments/files/27295688/00-START-HERE.md)
---
tags: [ctf, moc, index]
created: 2026-05-01
phase: 1
---

# 🚩 CTF Master Vault — เริ่มต้นที่นี่

> **Capture The Flag (CTF)** คือการแข่งขันด้านความปลอดภัยทางไซเบอร์ที่ผู้เล่นต้องหา "flag" (ข้อความรหัส เช่น `flag{...}`) ที่ซ่อนอยู่ในโจทย์ โดยใช้ทักษะการแฮก การวิเคราะห์ และการแก้ปัญหา

Vault นี้เป็นชุดความรู้ครบวงจรสำหรับเรียน CTF ตั้งแต่พื้นฐานจนถึงระดับสูง พร้อมอธิบาย **"ทำไมต้องทำแบบนี้"** ไม่ใช่แค่ "ทำยังไง"

---

## 📖 วิธีใช้ Vault นี้

1. **มือใหม่**: เริ่มที่ [[What-is-CTF]] → [[CTF-Types]] → [[Tools-Setup]] → [[Methodology]]
2. **มีพื้นฐานแล้ว**: เลือกหมวดที่อยากเก่ง แล้วไล่อ่านตามลำดับในหมวดนั้น
3. **กำลังแข่งจริง**: ไปที่ [[99-Cheatsheets/Quick-Reference|Quick Reference]] เพื่อดู payload สำเร็จรูป
4. ทุกหน้ามี `[[link]]` เชื่อมไปหน้าอื่น — กดเพื่อข้ามไปได้ทันที
5. ใช้ Graph View ของ Obsidian เพื่อดูภาพรวมความสัมพันธ์ของหัวข้อ

---

## 🎯 เฟสที่ 1 (ปัจจุบัน): พื้นฐาน + Web + Crypto

### 1️⃣ Fundamentals (พื้นฐาน)
- [[What-is-CTF|CTF คืออะไร?]]
- [[CTF-Types|ประเภทของ CTF]]
- [[Tools-Setup|เครื่องมือและการเซ็ตอัพ]]
- [[Methodology|วิธีคิดและขั้นตอนการแก้โจทย์]]

### 2️⃣ Reconnaissance (การลาดตระเวน)
- [[Passive-Recon|Passive Recon — เก็บข้อมูลแบบไม่แตะเป้าหมาย]]
- [[Active-Recon|Active Recon — สแกนและตรวจเป้าหมายตรงๆ]]
- [[OSINT-Techniques|OSINT — สืบจากข้อมูลสาธารณะ]]
- [[Enumeration|Enumeration — การ enumerate บริการต่างๆ]]

### 3️⃣ Web Exploitation
- [[SQL-Injection|SQL Injection — โจมตีฐานข้อมูล]]
- [[XSS|Cross-Site Scripting (XSS)]]
- [[CSRF|Cross-Site Request Forgery (CSRF)]]
- [[SSRF|Server-Side Request Forgery (SSRF)]]
- [[XXE|XML External Entity (XXE)]]
- [[LFI-RFI|Local/Remote File Inclusion]]
- [[Command-Injection|Command Injection]]
- [[Authentication-Bypass|Authentication Bypass]]
- [[JWT-Attacks|JWT Attacks]]
- [[SSTI|Server-Side Template Injection]]
- [[Deserialization|Insecure Deserialization]]
- [[Race-Conditions|Race Conditions]]
- [[IDOR|IDOR — Insecure Direct Object Reference]]

### 4️⃣ Cryptography
- [[Classical-Ciphers|รหัสคลาสสิก (Caesar, Vigenère, ...)]]
- [[Symmetric-Crypto|Symmetric Crypto (AES, DES)]]
- [[Asymmetric-Crypto|Asymmetric Crypto (RSA, ECC)]]
- [[Hash-Attacks|การโจมตีแฮช]]
- [[RSA-Attacks|RSA Attacks ละเอียด]]
- [[AES-Attacks|AES Attacks (Padding Oracle, ECB)]]

### 🛠 Cheatsheets
- [[Quick-Reference|Payload สำเร็จรูปสำหรับแข่ง]]
- [[Tools-Cheatsheet|คำสั่งเครื่องมือต่างๆ]]

---

## 🚧 เฟสที่ 2-3 (ทำต่อภายหลัง)

- Reverse Engineering
- Binary Exploitation (Pwn) — Buffer Overflow, ROP, Heap, Format String
- Forensics — Memory, Network, Disk, File Carving
- Steganography
- OSINT ขั้นสูง
- Mobile (Android/iOS)
- Hardware/IoT
- Cloud & Container Security
- Blockchain / Smart Contract
- AI/ML Security & Prompt Injection

---

## 🌐 แพลตฟอร์มฝึก CTF แนะนำ

| แพลตฟอร์ม | เหมาะกับ | URL |
|----------|---------|-----|
| **picoCTF** | มือใหม่สุด ฟรี มีแนะนำ | picoctf.org |
| **HackTheBox** | ทุกระดับ มีระบบจริงๆ | hackthebox.com |
| **TryHackMe** | มือใหม่ มี learning path | tryhackme.com |
| **CTFtime** | รวมการแข่งทั่วโลก + writeups | ctftime.org |
| **OverTheWire** | Linux/Web ขั้นพื้นฐาน | overthewire.org |
| **PortSwigger Web Academy** | Web ลึกที่สุด ฟรี | portswigger.net/web-security |
| **CryptoHack** | Crypto โดยเฉพาะ | cryptohack.org |
| **pwn.college** | Binary Exploitation ลึก | pwn.college |
| **Root Me** | ทุกหมวด ฝรั่งเศส/อังกฤษ | root-me.org |

---

## 🏷 Tags ที่ใช้ใน Vault นี้

- `#ctf` — ทุกไฟล์
- `#fundamentals` `#recon` `#web` `#crypto` `#pwn` `#rev` `#forensics` `#osint` — หมวดใหญ่
- `#tool` — เครื่องมือ
- `#payload` — payload สำเร็จรูป
- `#writeup` — writeup ตัวอย่าง
- `#cheatsheet` — cheatsheet

---

## 🎓 หลักคิดสำคัญ (อ่านก่อนเริ่ม!)

> **"การแฮกที่ดีเริ่มจากความเข้าใจ ไม่ใช่การจำ payload"**

CTF ไม่ใช่การจำ payload แล้วยิงไปเรื่อยๆ — มันคือการ **เข้าใจระบบลึกพอจะเห็นว่าตรงไหนพังได้** เพราะฉะนั้นทุกหน้าใน vault นี้จะอธิบาย:

1. **What** — มันคืออะไร
2. **Why** — ทำไมจึงพังได้ (root cause)
3. **How attack** — โจมตียังไง (with payloads)
4. **How detect** — ตรวจหายังไง
5. **How fix** — ป้องกันยังไง (สำคัญสำหรับเข้าใจลึก)

⚠️ **ข้อกฎหมาย/จริยธรรม**: ความรู้ใน vault นี้สำหรับ CTF, lab ส่วนตัว, หรือระบบที่ได้รับอนุญาต **เท่านั้น** การโจมตีระบบที่ไม่ได้รับอนุญาตเป็นอาชญากรรมในเกือบทุกประเทศ

---

#ctf #moc
