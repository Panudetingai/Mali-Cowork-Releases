<p align="center">
  <img src="./docs/brand/mali-cowork-icon.png" width="128" height="128" alt="Mali Cowork logo: yellow blob with two dark pill-shaped eyes" />
</p>

<h1 align="center">Mali Cowork</h1>

<p align="center">
  <strong>AI that works on your machine — not on someone else's server.</strong><br />
  <strong>AI ที่ทำงานบนเครื่องคุณ — ไม่ใช่บนเซิร์ฟเวอร์ของใคร</strong>
</p>

<p align="center">
  macOS · Windows &nbsp;·&nbsp; Chat for thinking &nbsp;·&nbsp; Cowork for real work on your files
</p>

<p align="center">
  <a href="https://github.com/Panudetingai/Mali-Cowork-Releases/releases/latest"><strong>⬇️ Download latest release / ดาวน์โหลด</strong></a>
  &nbsp;·&nbsp;
  <a href="https://github.com/Panudetingai/Mali-Cowork-Releases/issues/new/choose"><strong>🐞 Report a bug / แจ้งปัญหา</strong></a>
  &nbsp;·&nbsp;
  <a href="./docs/LANDING.md"><strong>📖 Docs / เอกสาร</strong></a>
</p>

<p align="center">
  🌐 Language / ภาษา: &nbsp; <a href="#english"><strong>English</strong></a> &nbsp;·&nbsp; <a href="#thai"><strong>ไทย</strong></a>
</p>

---

> This repository is **public** and contains **installers, documentation, and issue tracking only** — application source code lives in the private development repo. / เว็บนี้สำหรับ **ดาวน์โหลดตัวติดตั้ง อ่านเอกสาร และแจ้งปัญหา เท่านั้น** — โค้ดของโปรแกรมอยู่ในโปรเจกต์พัฒนาต่างหาก

---

<!-- ══════════════════════════════════════════════════════════════════ -->
<h2 id="english">English</h2>
<!-- ══════════════════════════════════════════════════════════════════ -->

### What is it

One desktop app for all the AI models and agents you already pay for. Pick a model once, then decide how much power it gets:

| Mode | For | Touches your files? |
|---|---|---|
| **Chat** | Q&A, writing, summarizing, thinking | ❌ No — never reads or edits files |
| **Cowork** | Agent edits code, organizes files, creates docs, runs commands | ✅ Yes — only in folders you approve, every action confirmable |

A chat stays in one mode forever — a plain chat can never silently become a file-editing agent.

### Download & Install

Get the installer from the [**Releases**](https://github.com/Panudetingai/Mali-Cowork-Releases/releases/latest) page:

| Your machine | File |
|---|---|
| macOS (Apple Silicon + Intel), macOS 10.13+ | `Mali Cowork_<version>_universal.dmg` |
| Windows 10/11 | `Mali Cowork_<version>_x64-setup.exe` |

**macOS**

1. Open the `.dmg` and drag **Mali Cowork** into **Applications**.
2. First open: the app is not notarized yet, so macOS may warn you — use one of:
   - **System Settings → Privacy & Security** → scroll down → **Open Anyway**
   - **Right click → Open** on the app
   - If it says the app is damaged, run in Terminal: `xattr -cr "/Applications/Mali Cowork.app"`
3. First time saving an API key, macOS asks for the password to access **Keychain** — enter it and press **Always Allow**.

**Windows**

1. Double-click `…_x64-setup.exe`.
2. If the blue *"Windows protected your PC"* screen appears, click **More info → Run anyway**.
3. Launch from the Start menu when done.

**First run**

1. The in-app setup helps you install the AI agent you need (e.g. OpenCode) step by step.
2. Add your API keys at **Settings → Models**, or use agents you already signed in to (Codex, Cursor, OpenCode…). Free models are included too.
3. Pick a mode: **Chat** to ask and think · **Cowork** to let the agent work — only in folders you approve.

> ⚠️ While the app is in early access, use Cowork on folders you have backed up (or git repos).

### Highlights

- **Every agent in one place** — local agents you already signed in to (**Claude Code**, Codex, OpenCode, Cursor Agent) and your own API keys (OpenAI, Anthropic, Google, xAI, DeepSeek, Mistral, Qwen, Z.ai, Kimi, OpenRouter, Groq). Switch mid-chat; subscriptions keep working.
- **Safe Cowork** — per-folder Read & write / Read only grants, permission cards before every action, **Undo/Redo every turn**, a Files-changed panel with line diff, plus a built-in Git panel and GitHub dashboard.
- **Work from your phone** — the phone remote, or your own **Telegram bot**: send tasks, approve actions in the chat, get results back. Share it safely with friends: allow-listed accounts + **daily token quota per friend** + task log.
- **Playbooks** — save tasks you run again and again (prompt + folder); start them from ⌘K or `/playbook` in Telegram.
- **Fix with Mali** — a failed GitHub Actions run gets a button: Mali opens a chat in your clone with the failing log, ready to fix.
- **Thai documents** — quotations, invoices, official letters as real `.docx`, with VAT 7% and Thai-words amounts computed for you.
- **Notch + Voice** — a pill at the top of the screen shows approvals and results while you work in another app; voice input and Quick Capture.
- **Private by default** — chat history in local SQLite, keys in Keychain / Credential Manager, no analytics, no telemetry, no Mali server.

### Security in 30 seconds

- Keys and tokens in **Keychain / Credential Manager** — never plain text in localStorage.
- Chat history in local **SQLite**, nothing uploaded anywhere.
- Folder allow-list enforced in the app itself; shell commands ask first; read-only folders are truly blocked.
- No analytics, no crash reporter, no account, no Mali server.

More honest answers about security are in the [security FAQ](./docs/LANDING.md).

### Report an issue

Use [**Issues → New issue**](https://github.com/Panudetingai/Mali-Cowork-Releases/issues/new/choose) — there are **Bug** and **Feature request** templates. Please include:

- Your OS and app version (e.g. macOS 15 / M2, Windows 11)
- What agent/model/feature you were using
- Steps to reproduce, and a screenshot or the error text

> 🔒 **Never paste API keys, passwords, or secret files into an issue.**

### Docs

| Doc | Covers |
|---|---|
| [LANDING.md](./docs/LANDING.md) | Full user guide in Thai + security FAQ |
| [INSTALL.md](./docs/INSTALL.md) | Step-by-step install guide (mostly Thai) |
| [FEATURES.md](./docs/FEATURES.md) | Feature list |
| [docs/README.md](./docs/README.md) | Index of all docs (including architecture notes) |

### Updates

- The app checks for updates on launch and every 6 hours. If auto-update doesn't offer it, download the new version from [Releases](https://github.com/Panudetingai/Mali-Cowork-Releases/releases/latest) and install over the old one.
- Uninstall: macOS — drag out of Applications · Windows — Settings → Apps → Uninstall.

---

<!-- ══════════════════════════════════════════════════════════════════ -->
<h2 id="thai">ไทย (ภาษาไทย)</h2>
<!-- ══════════════════════════════════════════════════════════════════ -->

### Mali Cowork คืออะไร

แอป desktop ตัวเดียวที่รวม **ทุกโมเดลและทุก agent ที่คุณจ่ายเงินไปแล้ว** เอาไว้ที่เดียว เลือกโมเดลครั้งเดียว แล้วคุณเป็นคนกำหนดว่าจะให้มันได้อำนาจมากแค่ไหน:

| โหมด | ใช้ทำอะไร | แตะไฟล์ได้ไหม |
|---|---|---|
| **Chat** | ถาม-ตอบ เขียนหนังสือ สรุปงาน คิดงาน | ❌ ไม่อ่าน ไม่แก้ไฟล์ใด ๆ |
| **Cowork** | agent แก้โค้ด จัดไฟล์ สร้างเอกสาร รันคำสั่ง | ✅ เฉพาะโฟลเดอร์ที่คุณกดอนุญาต ยืนยันทุกการกระทำ |

แชทหนึ่งอันจะอยู่โหมดเดียวตลอด — ไม่มีทางที่แชทธรรมดาจะกลายเป็น agent ที่แก้ไขไฟล์ได้กลางคัน

### ดาวน์โหลดและติดตั้ง

เลือกไฟล์ตามเครื่องจากหน้า [**Releases**](https://github.com/Panudetingai/Mali-Cowork-Releases/releases/latest):

| เครื่อง | ไฟล์ |
|---|---|
| macOS (ทั้ง Apple Silicon และ Intel), macOS 10.13 ขึ้นไป | `Mali Cowork_<เวอร์ชัน>_universal.dmg` |
| Windows 10/11 | `Mali Cowork_<เวอร์ชัน>_x64-setup.exe` |

**ติดตั้งบน macOS**

1. เปิดไฟล์ `.dmg` แล้วลาก **Mali Cowork** ไปใส่โฟลเดอร์ **Applications**
2. เปิดครั้งแรก: แอปยังไม่ได้ลงทะเบียนกับ Apple ระบบจึงอาจเตือน — ใช้วิธีใดวิธีหนึ่ง:
   - **System Settings → Privacy & Security** → เลื่อนลงล่าง → **Open Anyway** แล้วใส่รหัสผ่านเครื่อง
   - **คลิกขวา → Open** ที่ไอคอนแอป
   - ถ้าขึ้นว่าแอปเสียหาย ให้เปิด **Terminal** แล้วรันคำสั่งนี้:
     ```sh
     xattr -cr "/Applications/Mali Cowork.app"
     ```
3. ครั้งแรกที่บันทึก API key macOS จะถามรหัสผ่านเพื่อเข้าถึง **Keychain** — ใส่รหัสผ่านแล้วกด **Always Allow** (คีย์เก็บในเครื่องของคุณเท่านั้น)

**ติดตั้งบน Windows**

1. ดับเบิลคลิก `…_x64-setup.exe`
2. ถ้าขึ้นหน้าจอสีน้ำเงิน *"Windows protected your PC"* ให้กด **More info → Run anyway**
3. ทำตามขั้นตอนติดตั้งจนเสร็จ แล้วเปิดจากเมนู Start

**เริ่มใช้งานครั้งแรก**

1. เปิดแอปแล้วจะมี **หน้าตั้งค่าเริ่มต้น** ช่วยติดตั้ง AI agent ที่ต้องใช้ (เช่น OpenCode) ทำตามทีละขั้นได้เลย
2. ใส่ API key ที่ **Settings → Models** หรือใช้ agent ที่ล็อกอินไว้แล้วในเครื่อง (Codex, Cursor, OpenCode ฯลฯ) — มีโมเดลฟรีให้ด้วย
3. เลือกโหมด: **Chat** = ถามตอบ คิดงาน · **Cowork** = ให้ agent ทำงาน — เฉพาะในโฟลเดอร์ที่คุณอนุญาต

> ⚠️ ช่วงทดลอง (early access) แนะนำให้ใช้ Cowork กับโฟลเดอร์ที่มีสำรองไว้ หรือเป็น git repo

### จุดเด่น

- **ทุก agent รวมอยู่ที่เดียว** — agent ที่คุณล็อกอินไว้แล้ว (**Claude Code**, Codex, OpenCode, Cursor Agent) และ API key ของคุณ (OpenAI, Anthropic, Google, xAI, DeepSeek, Mistral, Qwen, Z.ai, Kimi, OpenRouter, Groq) สลับโมเดลกลางแชทได้ subscription ยังใช้ได้เหมือนเดิม
- **Cowork ที่ปลอดภัย** — ให้สิทธิเป็น Read & write / Read only แยกตามโฟลเดอร์ มี permission card ให้กดอนุมัติก่อนทุกอย่าง **Undo/Redo ย้อนได้ทุกเทิร์น** หน้า Files-changed ดู diff ทีละบรรทัด พร้อม Git panel และ GitHub dashboard
- **ทำงานจากมือถือ** — เข้าผ่าน phone remote หรือ **Telegram bot** ของคุณเอง: ส่งงาน อนุมัติในแชท รับผลลัพธ์กลับมา แชร์ให้เพื่อนได้อย่างปลอดภัย: allow-list บัญชี + **โควตา token ต่อเพื่อนรายวัน** + task log
- **Playbooks** — เก็บงานที่ทำซ้ำบ่อย (prompt + โฟลเดอร์) เรียกใช้จาก ⌘K หรือ `/playbook` ใน Telegram
- **Fix with Mali** — GitHub Actions ที่รันไม่ผ่านจะมีปุ่มให้กด: Mali เปิดแชทในโปรเจกต์ของคุณพร้อม log ที่ fail มาแก้ต่อเลย
- **เอกสารไทย** — ใบเสนอราคา ใบแจ้งหนี้ หนังสือราชการ ออกเป็นไฟล์ `.docx` จริง คำนวณ VAT 7% และจำนวนเงินอักษรไทยให้เรียบร้อย
- **Notch + เสียง** — pill ด้านบนจอแสดงการอนุมัติและผลลัพธ์ขณะทำงานในแอปอื่น พร้อมพิมพ์ด้วยเสียง และ Quick Capture
- **ส่วนตัวเป็นค่าเริ่มต้น** — ประวัติแชทเก็บใน SQLite บนเครื่อง คีย์อยู่ใน Keychain / Credential Manager ไม่มี analytics ไม่มี telemetry ไม่มีเซิร์ฟเวอร์ของ Mali

### ความปลอดภัยใน 30 วินาที

- คีย์และ token เก็บใน **Keychain / Credential Manager** — ไม่มีทางอยู่เป็น plain text ใน localStorage
- ประวัติแชทเก็บใน **SQLite** บนเครื่อง ไม่อัปโหลดขึ้นที่ไหน
- allow-list โฟลเดอร์บังคับในตัวแอปเอง คำสั่ง shell ถามก่อนเสมอ โฟลเดอร์ read-only ถูกบล็อกจริง
- ไม่มี analytics ไม่มี crash reporter ไม่มีบัญชี ไม่มีเซิร์ฟเวอร์ของ Mali

คำถามที่ควรถามเกี่ยวกับความปลอดภัย (ตอบตรง ๆ ทั้งที่ทำได้และทำไม่ได้): [FAQ ความปลอดภัย](./docs/LANDING.md)

### แจ้งปัญหา / ข้อเสนอแนะ

ใช้ [**Issues → New issue**](https://github.com/Panudetingai/Mali-Cowork-Releases/issues/new/choose) — มีเทมเพลต **Bug** และ **Feature request** ให้กรอกข้อมูลเหล่านี้:

- เครื่องและเวอร์ชัน OS (เช่น macOS 15 / M2, Windows 11) พร้อมเวอร์ชันแอป
- สิ่งที่กำลังใช้อยู่: agent/โมเดล/ฟีเจอร์ที่มีปัญหา
- ขั้นตอนที่ทำแล้วเกิดอะไรขึ้น ภาพหน้าจอหรือข้อความ error

> 🔒 **ห้ามแปะ API key, รหัสผ่าน หรือไฟล์ลับใน Issue เด็ดขาด**

### เอกสาร

| เอกสาร | เนื้อหา |
|---|---|
| [LANDING.md](./docs/LANDING.md) | คู่มือใช้งานเต็มภาษาไทย + ความปลอดภัย FAQ |
| [INSTALL.md](./docs/INSTALL.md) | คู่มือติดตั้งแบบละเอียดทีละขั้น |
| [FEATURES.md](./docs/FEATURES.md) | รายการฟีเจอร์ทั้งหมด |
| [docs/README.md](./docs/README.md) | ดัชนีเอกสารทั้งหมด (รวม architecture notes สำหรับผู้สนใจเทคนิค) |

### อัปเดตและถอนการติดตั้ง

- **อัปเดต:** แอปเช็กอัปเดตตอนเปิดโปรแกรมและทุก 6 ชม. ถ้าไม่มีเด้งมา ให้ดาวน์โหลดเวอร์ชันใหม่จาก [Releases](https://github.com/Panudetingai/Mali-Cowork-Releases/releases/latest) แล้วติดตั้งทับตัวเดิมได้เลย
- **ถอน:** macOS — ลากออกจาก Applications · Windows — Settings → Apps → Uninstall

---

## Repository scope / ขอบเขตของ repo นี้

| มีใน repo นี้ | ไม่มีใน repo นี้ |
|---|---|
| GitHub Releases (`.dmg`, `.exe`) | Source code |
| User & product documentation | Private keys / `.env` |
| Bug & feature issue templates | Internal CI secrets |

Releases are published here automatically when the private development repository tags a version. / ไฟล์ติดตั้งเผยแพร่ที่นี่โดยอัตโนมัติ หลังโปรเจกต์พัฒนา (เป็น repo private) ทำการแท็กเวอร์ชัน

---

<p align="center">
  <a href="https://github.com/Panudetingai/Mali-Cowork-Releases/releases/latest"><strong>⬇️ Download latest release / ดาวน์โหลดเวอร์ชันล่าสุด</strong></a>
</p>
