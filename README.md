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

## 🎯 ครบทุกหมวดของ CTF (เฟส 1+2+3)

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

### 5️⃣ Reverse Engineering
- [[RE-Intro|RE บทนำ — concept + tools stack]]
- [[Static-Analysis|Static Analysis — Ghidra, IDA, radare2]]
- [[Dynamic-Analysis|Dynamic Analysis — gdb, x64dbg, frida]]
- [[Assembly-Basics|Assembly Basics — x86_64 + ARM]]
- [[Anti-Debug-Tricks|Anti-Debug & Bypasses]]

### 6️⃣ Binary Exploitation (Pwn)
- [[Pwn-Intro|Pwn บทนำ — mitigations + pwntools]]
- [[Buffer-Overflow|Stack Buffer Overflow]]
- [[ROP|Return-Oriented Programming]]
- [[Format-String|Format String Vulnerability]]
- [[Heap-Exploitation|Heap Exploitation (glibc)]]
- [[Shellcoding|Shellcoding]]

### 7️⃣ Forensics
- [[Forensics-Intro|Forensics บทนำ]]
- [[Memory-Forensics|Memory Forensics — Volatility]]
- [[Network-Forensics|Network Forensics — Wireshark + pcap]]
- [[Disk-Forensics|Disk Forensics — Autopsy + Sleuth Kit]]

### 8️⃣ Steganography
- [[Stego-Intro|Stego บทนำ]]
- [[Image-Stego|Image Steganography — LSB, channels]]
- [[Audio-Stego|Audio Steganography — spectrogram, DTMF]]

### 🛠 Cheatsheets
- [[Quick-Reference|Payload สำเร็จรูปสำหรับแข่ง]]
- [[Tools-Cheatsheet|คำสั่งเครื่องมือต่างๆ]]

---

### 9️⃣ OSINT ขั้นสูง
- [[OSINT-Advanced|OSINT Advanced — image investigation, person tracking]]
- [[Geo-OSINT-Tricks|Geo-OSINT — เทคนิคระบุพิกัดจากภาพ]]

### 🔟 Mobile Security
- [[Mobile-Intro|Mobile บทนำ — APK/IPA structure]]
- [[Android-Reversing|Android Reversing — Frida hooks ลึก]]
- [[iOS-Hooking|iOS Hooking — class-dump + Frida]]

### 1️⃣1️⃣ Hardware & IoT
- [[Hardware-Intro|Hardware/IoT บทนำ — UART/JTAG/SDR]]
- [[Firmware-Analysis|Firmware Analysis — extract + emulate]]

### 1️⃣2️⃣ Cloud & Container
- [[Cloud-Security|Cloud Security — AWS/GCP/Azure misconfig]]
- [[Container-Security|Containers + Kubernetes — Docker escape, K8s RBAC]]

### 1️⃣3️⃣ Blockchain
- [[Smart-Contract-Security|Smart Contract Security — Solidity exploits]]
- [[Blockchain-Forensics|Blockchain Forensics — tx tracing, MEV]]

### 1️⃣4️⃣ AI/ML Security
- [[Prompt-Injection|Prompt Injection & LLM Attacks]]
- [[ML-Adversarial|ML Adversarial Attacks — adversarial examples]]

### 1️⃣5️⃣ Misc
- [[Misc-Challenges|Misc / Programming / Esoteric]]
- [[VM-Reversing|VM Reversing — custom bytecode disassembly]]

---

## ✅ Vault สมบูรณ์ครอบคลุมทุกหมวดของ CTF แล้ว!

หากต้องการลึกในจุดไหน บอกได้ — สามารถเขียน sub-pages เพิ่มเติม เช่น:
- เทคนิคเฉพาะ CVE หรือ challenge ดังๆ
- Writeup ของการแข่งจริง
- เครื่องมือเฉพาะที่อยากเจาะลึก

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
- หมวดใหญ่: `#fundamentals` `#recon` `#web` `#crypto` `#rev` `#pwn` `#forensics` `#stego` `#osint` `#mobile` `#hardware` `#iot` `#cloud` `#container` `#blockchain` `#ai` `#ml` `#misc`
- เฉพาะกลุ่ม: `#sql` `#xss` `#rsa` `#aes` `#gdb` `#ghidra` `#rop` `#heap` `#volatility` `#wireshark` `#lsb` `#frida` `#android` `#ios` `#docker` `#kubernetes` `#solidity` `#llm` `#prompt-injection` `#vm`
- `#tool` `#payload` `#cheatsheet` `#writeup`

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
