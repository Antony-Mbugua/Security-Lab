# security-labs


Practical, repeatable security labs with professional-grade writeups.


This repository is a curated collection of hands-on security labs I built and documented to demonstrate real-world red-team, blue-team, cloud, AD, and malware analysis skills. Each lab includes environment setup, attack/analysis steps, mitigations, detection guidance, and reproducible artifacts.


**Owner:** Antony Mbugua
**Portfolio:** https://antony-mbugua.github.io
**Handles:** HackTheBox: kiregi742 · TryHackMe: incog742


---


## Repo structure
security-labs/ ├─ README.md ├─ CONTRIBUTING.md ├─ labs/ │ ├─ 01-web-app-pentest/ │ │ ├─ README.md │ │ ├─ notes.md │ │ ├─ poc/ (scripts, exploit payloads) │ ├─ 02-owasp-top10/ │ ├─ 03-active-directory/ │ ├─ 04-siem-detection/ │ ├─ 05-cloud-iam/ │ ├─ 06-binary-exploitation/ │ ├─ 07-malware-analysis/ │ ├─ 08-api-security/ │ ├─ 09-containers-security/ │ ├─ 10-red-team-exercise/ │ ├─ 11-blue-team-response/ │ ├─ 12-combined-assessment/ ├─ tools/ (install scripts, docker-compose files) └─ assets/ (diagrams, screenshots, pcap files)

---


## How to use this repo


1. Clone this repo.
2. Read the top-level README for the week-by-week roadmap.
3. For each lab folder, follow its `README.md` to spin up the environment (Docker, Vagrant, or VM), execute the lab, and produce a writeup.
4. Commit work in feature branches (`lab/01-web-app-pentest`) and open a PR; use the rubric in this repo to grade your own work.


---


## Grading rubric (quick)
- Reproducibility: 1–5
- Depth: 1–5
- Analysis: 1–5
- Presentation: 1–5


Target: **≥16/20** for portfolio-quality labs.


---


## TL;DR for recruiters
Pick 2–3 labs labeled `portfolio-ready` and read the executive summary at the top of each. Each lab contains a short TL;DR so you can decide if you want the technical report.


---


## License & responsible disclosure
This repository is intended for educational purposes only. Do not upload or include malware samples, stolen data, or credentials. Red-team activities must be performed in isolated lab networks under your control. If you discover a real-world vulnerability while doing research, follow a responsible disclosure policy and do not publish exploit code for active, unpatched systems.
---



