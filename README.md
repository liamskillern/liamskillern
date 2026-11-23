<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=700&size=30&duration=3500&pause=1200&color=D4AF37&center=true&vCenter=true&width=700&height=60&lines=Hi%2C+I'm+Liam;Cybersecurity+student+%40+CSU+Pueblo;Keeper+of+a+Homelab;One+SIEM+to+watch+them+all" alt="Typing intro" />

*Not all who tinker are lost.*

I'm most interested in how things break: vulnerabilities, attacks, and how to catch them.<br/>
Most of what I learn, I learn by building it in my homelab first.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/liam-skillern/)
[![GitHub](https://img.shields.io/badge/GitHub-1B1B1B?style=for-the-badge&logo=github&logoColor=D4AF37)](https://github.com/liamskillern)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/liamskill/)
[![X](https://img.shields.io/badge/X-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/liamskillern_)
![Based in Colorado](https://img.shields.io/badge/Based_in-Fort_Collins,_CO-3B5D3A?style=for-the-badge)

</div>

---

<h2 align="center"><img src="assets/fellowship-banner.svg" alt="⚔️ The Fellowship of Skills" width="100%" /></h2>

**🛡️ Defense and detection**<br/>
![Wazuh](https://img.shields.io/badge/Wazuh_SIEM-3595F9?style=flat-square&logo=wazuh&logoColor=white)
![Nessus](https://img.shields.io/badge/Nessus-00C176?style=flat-square&logo=tenable&logoColor=white)
![AdGuard Home](https://img.shields.io/badge/AdGuard_Home-68BC71?style=flat-square&logo=adguard&logoColor=white)
![Uptime Kuma](https://img.shields.io/badge/Uptime_Kuma-5CDD8B?style=flat-square&logo=uptimekuma&logoColor=white)

**🗡️ Offense**<br/>
![Kali Linux](https://img.shields.io/badge/Kali_Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white)
![Active Directory attacks](https://img.shields.io/badge/Active_Directory_attacks-0078D4?style=flat-square&logo=windows&logoColor=white)

**🏰 Systems and infrastructure**<br/>
![Ubuntu](https://img.shields.io/badge/Ubuntu_Server-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows_Server_2025-0078D4?style=flat-square&logo=windows&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)
![VMware](https://img.shields.io/badge/VMware_Workstation-607078?style=flat-square&logo=vmware&logoColor=white)
![Tailscale](https://img.shields.io/badge/Tailscale-242424?style=flat-square&logo=tailscale&logoColor=white)
![Nextcloud](https://img.shields.io/badge/Nextcloud-0082C9?style=flat-square&logo=nextcloud&logoColor=white)

**🔮 AI**<br/>
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=flat-square&logo=claude&logoColor=white)
![Prompt injection defense](https://img.shields.io/badge/Prompt_injection_defense-8B0000?style=flat-square)

---

## 🗺️ Quests in Progress

| Quest | What it is | Status |
|---|---|---|
| 🏰 **Active Directory lab** | Build it, attack it, detect it. A Windows Server 2025 domain controller, a Kali attacker, Wazuh for detection and Nessus for scanning. | 🟡 Write-up coming |
| 🌋 **[Homelab](https://github.com/liamskillern/homelab)** | An Ubuntu server I run myself, with a Wazuh SIEM watching every machine I own. Map below, full write-up [here](https://github.com/liamskillern/homelab). | 🟢 Running |
| 🔮 **Ultron, my AI morning brief** | Claude Code reads my email and calendar and writes me a daily brief. See *The Palantír* below. | 🟡 Moving to the cloud |
| 🛡️ **FOCO Cyber** | Security help for small businesses in Fort Collins. | 🟡 Starting up |

---

## 🌍 Map of my Middle-earth (the homelab)

Everything is reached over Tailscale, so nothing is exposed to the open internet. The full tour lives in my [homelab repo](https://github.com/liamskillern/homelab).

<div align="center">
  <img src="assets/homelab-map.svg" alt="Map of my homelab. My desktop, laptop and Pixel 9 connect over Tailscale to my Ubuntu server running Nextcloud, Immich, Paperless, AdGuard Home, Uptime Kuma and Wazuh SIEM. A VMware AD lab has Kali and Nessus targeting a Windows Server 2025 domain controller. Wazuh agents report to the SIEM." width="100%" />
</div>

---

## 🔮 The Palantír (what I'm building with Claude)

<div align="center">
  <img src="assets/palantir.svg" alt="An animated palantir showing visions of Ultron at work, next to a diagram: email and calendar pass through a read-only tool allowlist to Claude Code, which writes a daily brief and pings my Pixel. Orders hidden in emails are blocked." width="100%" />
</div>

I'm learning to use Claude Code well, and I treat it like a security problem as much as a coding tool.

- **Ultron** runs on a schedule, reads my email and calendar, writes a daily brief to my notes, and pings my phone.
- **Read-only by design.** An agent that reads email is a prompt-injection target, because anyone who emails me can try to give it orders. So it only gets read-only tools, and everything it reads is data, never instructions.
- **This profile** was designed by me and built with Claude Code, down to the maps.

> *Even the very wise cannot see all ends. That's why the agent doesn't get write access.*

---

## 📜 The Road to Security+

<div align="center">
  <img src="assets/security-plus-map.svg" alt="Map of my Security+ journey: from the Shire through Rivendell, Moria, Helm's Deep, Minas Tirith and Edoras (the five exam domains) to Mount Doom (the exam). Domains 1 and 2 are done and I'm at Helm's Deep, domain 3." width="100%" />
</div>

Each stop is one of the five CompTIA Security+ (SY0-701) exam domains. Mount Doom is the exam itself, target **summer 2027**.

<details>
<summary>The domains as a checklist</summary>

- [x] 1. General Security Concepts (Rivendell)
- [x] 2. Threats, Vulnerabilities, and Mitigations (Moria)
- [ ] 3. Security Architecture (Helm's Deep)
- [ ] 4. Security Operations (Minas Tirith)
- [ ] 5. Security Program Management and Oversight (Edoras)

</details>

---

## 🧭 Seeking a Fellowship

<div align="center">
  <img src="assets/seeking-fellowship.svg" alt="Seeking a Fellowship. Education: B.S. Cybersecurity at CSU Pueblo (graduating Winter 2027), A.S. Cybersecurity from Arapahoe Community College, Security+ in progress. Looking for internships and entry-level roles in cybersecurity, IT and help desk, and AI. Experience: FOCO Cyber founder, homelab administrator, Wazuh SIEM and detection, Active Directory attack lab, AI automation with Claude Code." width="100%" />

<br/>

[![Hire me: message me on LinkedIn](https://img.shields.io/badge/Hiring%3F_Message_me_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/liam-skillern/)

</div>

---

<div align="center">

## 📊 Deeds recorded in the Red Book

<img src="https://github-readme-stats.vercel.app/api?username=liamskillern&show_icons=true&theme=gruvbox&hide_border=true" alt="GitHub stats" height="165" />
<img src="https://streak-stats.demolab.com?user=liamskillern&theme=gruvbox&hide_border=true" alt="GitHub streak" height="165" />

*The road goes ever on.*

</div>
