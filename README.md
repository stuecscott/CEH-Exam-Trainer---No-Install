# CEH-Exam-Trainer---No-Install
AI-powered CEH exam trainer, 186 questions across all 12 domains with detailed answer explanations and unlimited Claude-generated practice questions. No install required.

# 🔐 CEH Master Exam Trainer

An AI-powered, browser-based **Certified Ethical Hacker (CEH)** exam preparation tool with **186 hand-crafted questions** across all 12 CEH exam domains — plus unlimited AI-generated bonus questions powered by Claude. No installation, no server, no account required.

> Part of an open-source cybersecurity study toolkit. See all tools at the bottom of this page.

---

## 📖 Based On

- **CEH Certified Ethical Hacker Practice Exams, Fourth Edition** — Matt Walker (McGraw-Hill)
- **EC-Council CEH v12 Exam Objectives**
- Real-world ethical hacking concepts and tools tested on the 125-question CEH exam

---

## 🚀 Getting Started

### Option 1 — Open directly in your browser
```bash
git clone https://github.com/YOUR-USERNAME/ceh-master-trainer.git
cd ceh-master-trainer
open ceh_exam_trainer.html        # macOS
# or double-click the file in File Explorer (Windows/Linux)
```

### Option 2 — GitHub Pages (live hosted URL)
1. Fork this repository
2. Go to **Settings → Pages → Deploy from main branch**
3. Your trainer is live at: `https://YOUR-USERNAME.github.io/ceh-master-trainer/`

### Option 3 — Use directly in Claude
Upload `ceh_exam_trainer.html` to a Claude conversation, or share your GitHub Pages URL and ask Claude to run it.

---

## 📚 Question Bank — 186 Questions + Unlimited AI

| # | Domain | Questions | Topics Covered |
|---|--------|-----------|----------------|
| 1 | Ethical Hacking Essentials | 24 | CEH methodology, attack phases, risk, legal concepts |
| 2 | Reconnaissance & Footprinting | 19 | OSINT, Google hacking, WHOIS, DNS, Maltego, Shodan |
| 3 | Scanning & Enumeration | 19 | Nmap flags/scans, NetBIOS, SNMP, banner grabbing, NSE |
| 4 | Sniffing & Evasion | 14 | Wireshark, ARP spoofing, MAC flooding, IDS evasion |
| 5 | System Hacking | 15 | Password attacks, privilege escalation, lateral movement |
| 6 | Malware & Trojans | 13 | RATs, ransomware, rootkits, C2, polymorphic malware |
| 7 | Wireless Hacking | 13 | WEP/WPA/WPA3, Aircrack-ng, evil twin, deauth attacks |
| 8 | Web Application Attacks | 15 | SQLi, XSS, CSRF, SSRF, XXE, OWASP Top 10 |
| 9 | Cryptography | 14 | Symmetric/asymmetric, PKI, hashing, TLS, PFS |
| 10 | Social Engineering | 13 | Phishing, pretexting, tailgating, vishing, baiting |
| 11 | DoS & Session Hijacking | 12 | DDoS types, SYN flood, amplification, session theft |
| 12 | Cloud & IoT Security | 15 | Cloud models, FedRAMP, misconfiguration, containers |
| | **Total** | **186** | |

Every question screen also includes a **Generate AI Question** button powered by Claude — fresh exam-quality questions on any domain, unlimited.

---

## 🛠 Features

### Study Mode vs Exam Mode
- **📚 Study Mode** — Hints available before answering; full explanation after every answer. Best for learning.
- **⏱ Exam Mode** — No hints, simulates real CEH exam pressure. Best for self-assessment.

### Detailed Answer Explanations
Every question includes why the correct answer is right AND why each wrong answer is wrong — so you never accidentally reinforce incorrect knowledge from distractor choices.

### Domain Filtering
Click any of the 12 domain buttons in the sidebar to focus on one area, or run a full mixed exam across all domains.

### Live Score Tracking
Running Correct / Wrong / Total / Percentage throughout the session. End-of-session results screen with grade and study guidance.

---

## 🎯 CEH Exam Overview

| Item | Detail |
|------|--------|
| Certification | Certified Ethical Hacker (CEH) |
| Issuing body | EC-Council |
| Questions | 125 multiple choice |
| Duration | 4 hours |
| Passing score | ~70% (varies by exam form) |
| Delivery | Pearson VUE proctored |

### CEH Attack Methodology — Memorize This
```
1. Reconnaissance  (Footprinting / OSINT)
2. Scanning & Enumeration
3. Gaining Access  (Exploitation)
4. Maintaining Access  (Persistence / Rootkits / Zombies)
5. Covering Tracks  (Clear logs / Timestomping)
```

### Key Tools Covered

| Category | Tools |
|----------|-------|
| Scanning | Nmap, Hping3, Zenmap |
| Enumeration | enum4linux, Netcat, snmpwalk |
| Sniffing / MITM | Wireshark, Ettercap, tcpdump |
| Web App Testing | Burp Suite, sqlmap, Nikto |
| Wireless | Aircrack-ng, Kismet, Reaver |
| Password / Credentials | John the Ripper, Hashcat, Mimikatz |
| OSINT / Recon | Maltego, theHarvester, Shodan |
| Exploitation | Metasploit Framework |

---

## 📁 File Structure

```
ceh-master-trainer/
│
├── ceh_exam_trainer.html    # Complete application — single self-contained file
└── README.md                # This file
```

Everything — 186 questions, all CSS, JavaScript, and AI integration — is in one HTML file. No dependencies, no build process.

---

## 🤝 Contributing

To add questions, use this format in the `QUESTION_BANK` array inside `ceh_exam_trainer.html`:

```javascript
{
  topic: 0,              // 0-11 matching the 12 domains above
  diff: 'medium',        // 'easy' | 'medium' | 'hard'
  type: 'Multiple Choice',
  q: 'Question text here',
  opts: ['Option A', 'Option B', 'Option C', 'Option D'],
  ans: 0,                // index of correct answer (0-3)
  hint: 'A hint that guides without giving the answer',
  correct_fb: 'Why the correct answer is right. Use <strong> tags for key terms.',
  wrong_fb:   'Why wrong answers fail, and why the correct answer is right.'
}
```

**Ideas for future contributions:**
- [ ] More questions toward 25+ per domain
- [ ] Timed 125-question full mock exam mode
- [ ] Weak domain tracking across sessions
- [ ] Tool identification from command output questions
- [ ] Export wrong answers as a review list

---

## ⚠️ Disclaimer

For educational purposes only to assist with CEH exam preparation. All hacking techniques described are for defensive knowledge and authorized testing only. Never apply these techniques against systems you do not have explicit written permission to test.

---

## 🔗 Full Cybersecurity Study Toolkit

This trainer is part of a growing open-source collection. All tools are single HTML files — no install required.

| Tool | Description | Size |
|------|-------------|------|
| [🌐 CCNA Subnet Reference Tool](https://github.com/YOUR-USERNAME/ccna-subnet-tool) | Interactive subnetting calculator + VLAN planner + block size/mask reference grid | Single HTML |
| [🎓 CCNA Master Exam Trainer](https://github.com/YOUR-USERNAME/ccna-master-trainer) | CCNA exam prep across all 8 exam domains with AI generation | 288 questions |
| [🔐 CEH Master Exam Trainer](https://github.com/YOUR-USERNAME/ceh-master-trainer) | CEH exam prep across all 12 exam domains with AI generation | 186 questions |

Replace `YOUR-USERNAME` with your GitHub username. All three tools can also be used directly in Claude by uploading the HTML file or sharing the GitHub Pages URL.

---

## 📄 License

MIT License — free to use, modify, and share. Attribution appreciated but not required.

---

*No install. No login. No ads. Open the file and study.*
