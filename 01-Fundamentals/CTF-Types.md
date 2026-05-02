---
tags: [ctf, fundamentals]
created: 2026-05-01
---

# ประเภทของ CTF

CTF มี **3 รูปแบบหลัก** ที่ต่างกันอย่างชัดเจน บวกกับ **หมวดโจทย์** อีกหลายแบบ

---

## 🎯 รูปแบบการแข่ง (Format)

### 1. Jeopardy-style ⭐ (พบบ่อยที่สุด)
- มีโจทย์แยกเป็นหมวด (Web, Crypto, Pwn, ฯลฯ) เหมือนกระดานเกมโชว์ "Jeopardy!"
- แต่ละข้อมีคะแนน ยากมาก = คะแนนสูง
- ทีมไหนได้คะแนนรวมสูงสุดในเวลาที่กำหนด ชนะ
- **ตัวอย่าง**: picoCTF, Google CTF, DefCon Quals

```
┌──────┬──────┬──────┬──────┐
│ Web  │Crypto│ Pwn  │ Rev  │
├──────┼──────┼──────┼──────┤
│ 100  │ 100  │ 100  │ 100  │
│ 200  │ 200  │ 200  │ 200  │
│ 500  │ 500  │ 500  │ 500  │
└──────┴──────┴──────┴──────┘
```

### 2. Attack-Defense (A/D)
- แต่ละทีมได้ **server เหมือนกัน** ที่มีบริการมีช่องโหว่
- ต้อง **patch ของตัวเอง** + **โจมตีของคนอื่น** เพื่อขโมย flag
- ระบบ check ว่าบริการยังทำงานอยู่ไหม (ถ้าปิดถูกหักคะแนน)
- ยากมาก ใช้กับการแข่งระดับสูง เช่น DefCon Finals, iCTF

```
[Team A server] ← attacks ← [Team B]
       ↓
   ขโมย flag จาก Team A
```

**กลยุทธ์สำคัญ**:
- หา 0-day ในบริการที่จัดมาให้ก่อนคนอื่น
- Patch ช่องโหว่เร็วๆ แต่ไม่ break service
- Monitor traffic ของตัวเอง เพื่อรู้ว่าโดนโจมตีด้วยอะไร แล้วเอาวิธีนั้นไปใช้กับคนอื่น (replay)

### 3. King of the Hill (KoTH)
- ทุกทีมแย่งคุมระบบเดียวกัน
- ใครคุมไว้ได้นานที่สุด ชนะ
- พบในงานเล็กๆ บางครั้งใน HTB

### 4. Mixed / Boot2Root
- โจทย์เป็น "เครื่อง" ที่ต้องแฮกเข้าจาก user → root
- คล้ายงานจริง เริ่มจาก scan → exploit → privilege escalation
- ตัวอย่าง: HackTheBox, VulnHub

---

## 📚 หมวดโจทย์ (Categories)

### 🌐 Web Exploitation
โจมตีเว็บแอป — เป็นหมวดที่นิยมและเข้าใจง่ายสุดสำหรับมือใหม่

หัวข้อย่อย: [[SQL-Injection]], [[XSS]], [[CSRF]], [[SSRF]], [[XXE]], [[LFI-RFI]], [[Command-Injection]], [[JWT-Attacks]], [[SSTI]], [[Deserialization]], [[IDOR]], [[Race-Conditions]]

### 🔐 Cryptography (Crypto)
ถอดรหัส โจมตี algorithm — ต้องใช้คณิตศาสตร์

หัวข้อย่อย: [[Classical-Ciphers]], [[Symmetric-Crypto]], [[Asymmetric-Crypto]], [[RSA-Attacks]], [[Hash-Attacks]], [[AES-Attacks]]

### 🔧 Reverse Engineering (Rev)
แกะ binary/program เพื่อเข้าใจว่ามันทำอะไร และหา flag ในนั้น

เครื่องมือหลัก: Ghidra, IDA Pro, Binary Ninja, radare2, gdb

### 💥 Binary Exploitation (Pwn)
โจมตี binary โดยใช้ memory corruption เช่น buffer overflow → ROP → shell

เครื่องมือหลัก: gdb + pwndbg/gef, pwntools (Python), ROPgadget, checksec

### 🕵️ Forensics
สืบหาหลักฐานจาก:
- Memory dumps (Volatility)
- Network captures (Wireshark, .pcap files)
- Disk images (Autopsy, Sleuth Kit)
- Files ต่างๆ (file carving, hex analysis)

### 🖼 Steganography (Stego)
ซ่อนข้อมูลในไฟล์อื่น — รูปภาพ, เสียง, วิดีโอ
- LSB (Least Significant Bit) ในรูป
- Spectrogram ในเสียง
- Metadata ในไฟล์

เครื่องมือ: steghide, zsteg, stegsolve, exiftool, binwalk, sonic-visualiser

### 🌍 OSINT (Open-Source Intelligence)
สืบจากข้อมูลสาธารณะ — Google, Twitter, Shodan, Wayback Machine, ภาพถ่าย, metadata

### 📱 Mobile
APK (Android) หรือ IPA (iOS) — มักรวม reverse + crypto + web

### 🔌 Hardware / IoT
Firmware analysis, embedded systems, signal analysis (radio, electronics)

### ☁️ Cloud / Container
AWS misconfiguration, Kubernetes, Docker escape, IAM privilege escalation

### ⛓ Blockchain / Smart Contract
Solidity bugs, reentrancy, integer overflow, flash loan attacks

### 🤖 AI/ML Security (ใหม่)
Prompt injection, jailbreak, model extraction, adversarial examples
> ตามรายงานปี 2025-2026 หมวดนี้เพิ่มขึ้นมากในงานแข่งใหญ่

### 🎨 Misc (อื่นๆ)
รวมโจทย์ที่ไม่เข้าหมวดไหน — programming, esoteric, puzzle, etc.

---

## เลือกหมวดอะไรเริ่มก่อน?

| ระดับ | แนะนำหมวด | เหตุผล |
|------|----------|--------|
| **มือใหม่สุด** | Web, Crypto (classical), OSINT, Misc | ไม่ต้องเขียนโค้ดมาก ใช้ tool ผ่าน browser ได้ |
| **มีพื้น Linux** | Forensics, Stego | ใช้คำสั่ง CLI เป็นหลัก |
| **เขียนโค้ดได้** | Rev (เริ่มจาก Ghidra) | ต้องอ่าน assembly/decompile |
| **มี OS/C ขั้นสูง** | Pwn | ต้องเข้าใจ memory, stack, heap ลึก |

> 💡 ผู้เขียนแนะนำให้เริ่มที่ **Web** + **Crypto classical** เพราะแฟลตชัน learning curve ดีและเห็นผลเร็ว

---

## 🔗 ต่อไป

- เลือกแล้วไปเซ็ตอัพเครื่องที่ [[Tools-Setup]]
- เรียน [[Methodology|วิธีคิดและขั้นตอนการแก้โจทย์]]
- กลับ [[00-START-HERE|หน้าหลัก]]

---

#ctf #fundamentals
