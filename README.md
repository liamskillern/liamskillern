<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Cinzel&weight=700&size=30&duration=3500&pause=1200&color=D4AF37&center=true&vCenter=true&width=700&height=60&lines=Hi%2C+I'm+Liam;Cybersecurity+student+%40+CSU+Pueblo;Keeper+of+a+homelab+in+Colorado;One+SIEM+to+watch+them+all" alt="Typing intro" />

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

## ⚔️ The Fellowship of Skills

> *Every quest needs a company. These are mine.*

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

```mermaid
flowchart LR
    subgraph Shire["🏡 My devices"]
        PC["🖥️ Desktop (built it myself)"]
        Laptop["💻 Laptop"]
        Phone["📱 Pixel 9"]
    end

    TS{{"🧝 Tailscale<br/>private network"}}

    subgraph MinasTirith["🏰 Ubuntu server"]
        NC["☁️ Nextcloud"]
        IM["🖼️ Immich"]
        PL["📄 Paperless"]
        AG["🚫 AdGuard Home"]
        UK["📈 Uptime Kuma"]
        WZ["👁️ Wazuh SIEM"]
    end

    subgraph Mordor["🌋 AD attack lab (VMware)"]
        DC["🪟 Windows Server 2025 DC"]
        KALI["🐉 Kali attacker"]
        NS["🔎 Nessus"]
    end

    PC & Laptop & Phone --> TS --> MinasTirith
    KALI -- attacks --> DC
    NS -- scans --> DC
    PC & Laptop & DC -. Wazuh agents .-> WZ
```

---

## 🔮 The Palantír (what I'm building with Claude)

I'm learning to use Claude Code well, and I'm treating it like a security problem as much as a coding tool.

- **Ultron morning brief.** Claude Code runs on a schedule, reads my email and calendar, and writes a daily brief to my notes, then pings my phone.
- **Read-only by design.** An agent that reads email is a prompt-injection target: anyone who emails me can try to give it orders. So it only gets an allowlist of read-only tools, and it treats everything it reads as data, never as instructions.
- **This profile.** Designed by me, built with Claude Code, merged through a pull request.

> *Even the very wise cannot see all ends. That's why the agent doesn't get write access.*

---

## 📜 The Road to Security+

Target: **summer 2027**, CompTIA Security+ (SY0-701). I check off each domain as I finish it.

![Progress](https://img.shields.io/badge/Domains_done-0%20of%205-D4AF37?style=for-the-badge)

- [ ] 1. General Security Concepts
- [ ] 2. Threats, Vulnerabilities, and Mitigations
- [ ] 3. Security Architecture
- [ ] 4. Security Operations
- [ ] 5. Security Program Management and Oversight

---

## 🧭 Seeking a Fellowship

I'm looking for **internships and entry-level roles** in:

- 🛡️ **Cybersecurity:** SOC analyst, security operations
- 🖥️ **IT and help desk:** desktop support, systems administration
- 🔮 **AI:** AI operations, automation, and securing AI agents

- 🎓 B.S. Cybersecurity, **CSU Pueblo**, graduating Winter 2027
- 🎓 A.S. Cybersecurity, **Arapahoe Community College**
- 📍 Fort Collins, Colorado, open to remote

If you're hiring, [message me on LinkedIn](https://www.linkedin.com/in/liam-skillern/).

---

<div align="center">

## 📊 Deeds recorded in the Red Book

<img src="https://github-readme-stats.vercel.app/api?username=liamskillern&show_icons=true&theme=gruvbox&hide_border=true" alt="GitHub stats" height="165" />
<img src="https://streak-stats.demolab.com?user=liamskillern&theme=gruvbox&hide_border=true" alt="GitHub streak" height="165" />

*The road goes ever on.*

</div>
