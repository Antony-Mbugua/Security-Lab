# security-labs

**Practical, repeatable security labs with professional-grade writeups.**

This repository is a curated collection of hands-on security labs I built and documented to demonstrate real-world **red-team, blue-team, cloud, Active Directory, and malware analysis** skills.  

Each lab includes:
- **Environment setup**
- **Attack/analysis steps**
- **Mitigations**
- **Detection guidance**
- **Reproducible artifacts**

---

## 📌 Owner & Portfolio
- **Owner:** Antony Mbugua  
- **Portfolio:** [antony-mbugua.github.io](https://antony-mbugua.github.io)  
- **Handles:**  
  - HackTheBox: **`kiregi742`**  
  - TryHackMe: **`incog742`**  

---

## 📂 Repo Structure
```yaml
security-labs/
├─ README.md
├─ CONTRIBUTING.md
├─ labs/
│  ├─ 01-web-app-pentest/
│  │  ├─ README.md
│  │  ├─ notes.md
│  │  ├─ poc/ (scripts, exploit payloads)
│  ├─ 02-owasp-top10/
│  ├─ 03-active-directory/
│  ├─ 04-siem-detection/
│  ├─ 05-cloud-iam/
│  ├─ 06-binary-exploitation/
│  ├─ 07-malware-analysis/
│  ├─ 08-api-security/
│  ├─ 09-containers-security/
│  ├─ 10-red-team-exercise/
│  ├─ 11-blue-team-response/
│  ├─ 12-combined-assessment/
├─ tools/   (install scripts, docker-compose files)
└─ assets/  (diagrams, screenshots, pcap files)

**## 🚀 How to Use This Repo**
Clone this repo:

bash
Copy code
git clone https://github.com/Antony-Mbugua/security-labs.git
cd security-labs
Read this top-level README for the week-by-week roadmap.

For each lab folder:

Open its README.md

Spin up the environment (Docker, Vagrant, or VM)

Execute the lab

Document your findings

Commit work in feature branches (e.g., lab/01-web-app-pentest) and open a PR.
Use the rubric below to grade your own work.


**📝 Grading Rubric (Quick)**
Reproducibility: 1–5

Depth: 1–5

Analysis: 1–5

Presentation: 1–5

**🎯 Target: ≥ 16/20 → portfolio-quality labs.**

**🎯 TL;DR for Recruiters**
Check labs tagged portfolio-ready

Each has an executive summary at the top

Read summaries first; dive into full technical reports if relevant

**⚖️ License & Responsible Disclosure**
This repository is intended for educational purposes only.

🚫 Do not upload or include:

Malware samples

Stolen data

Credentials

Red-team activities must be performed in isolated lab networks under your control.

If you discover a real-world vulnerability while doing research:

Follow a responsible disclosure policy

Do not publish exploit code for active, unpatched systems
