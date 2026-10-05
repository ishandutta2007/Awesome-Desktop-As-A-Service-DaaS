# Awesome-Desktop-As-A-Service-DaaS

# Awesome-Desktop-As-A-Service-DaaS



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Cloud PCs, Virtual Desktop Infrastructure (VDI), Application Streaming & Remote Access*

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Desktop as a Service (DaaS)**. These tools help organizations deliver virtual desktops, applications, and secure browsers to any device through a web browser—centralizing control, improving security, and supporting distributed workforces.



**Examples** include Windows 365 (Cloud PC), Amazon WorkSpaces, Citrix DaaS, Omnissa Horizon Cloud, Azure Virtual Desktop, Dizzion Frame, Kasm Workspaces, Apache Guacamole, IsardVDI, and RustDesk (the category leaders).



**Open-source emphasis**: The open-source DaaS ecosystem is **exceptionally mature and production-proven**. **Kasm Workspaces** delivers browser-based containers, applications, and desktops with GPU acceleration, Zero Trust integration via OpenZiti, and native Proxmox VE support . **Apache Guacamole** is the de-facto clientless remote desktop gateway supporting VNC, RDP, and SSH through a browser . **IsardVDI** provides a free KVM-based desktop virtualization platform with GPU support and Docker deployment . **RustDesk** offers a self-hosted remote desktop alternative with full data control . This section documents these production-grade solutions.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## 📖 Table of Contents



- [☁️ SaaS/Hosted Platforms](#-saas-hosted-platforms)

- [🔓 Open-Source GitHub Projects](#-open-source-github-projects)

- [🤝 How to Contribute](#-how-to-contribute)

- [⚠️ Disclaimer](#-disclaimer)



## ☁️ SaaS/Hosted Platforms



> **📊 Market Context**: The global Desktop-as-a-Service market is estimated at **~$8B in 2026**, growing toward **~$25B by 2032** at a **~20% CAGR**. The sector is **moderately concentrated** — **Citrix** and **Omnissa** (formerly VMware Horizon) dominate enterprise VDI, while **Microsoft** offers both **Azure Virtual Desktop** (flexible, consumption-based) and **Windows 365** (simpler, fixed per-user Cloud PC) . **Pricing varies dramatically**: Windows 365 Business Basic starts at **$28/user/month** (2 vCPU/4 GB) , Amazon WorkSpaces publishes a **$25/month Windows Value example** , and Citrix DaaS uses **quote-based or calculator pricing** . No single vendor holds a winner-take-all position; enterprises typically run hybrid DaaS + VDI stacks.



| Platform | Description | Pricing (Starting Tier) | Free Tier Limits | Company Size |

|----------|-------------|------------------------|------------------|--------------|

| **[Windows 365 (Cloud PC)](https://www.microsoft.com/en-us/windows-365)** | **Persistent Cloud PC with one-user, one-desktop model.** Predictable monthly pricing, deep integration with Microsoft 365, Entra ID, and Intune. | **Business Basic**: **$28/user/month** (2 vCPU/4 GB); **Standard**: **$36** (2 vCPU/8 GB); **Premium**: **$56** (4 vCPU/16 GB). 128 GB storage included . | **None** — 30-day trial available via Microsoft 365 trial. **No perpetual free tier**. | **~$281B revenue (Microsoft FY2025)** |

| **[Azure Virtual Desktop](https://azure.microsoft.com/en-us/products/virtual-desktop/)** | **Microsoft's flexible cloud VDI.** Multi-session Windows 10/11, RemoteApp streaming, and consumption-based pricing. | **Consumption-based**: Pay for compute (VM hours) + storage + networking. No per-user license fee for multi-session Windows . | **None** — Azure free account gives $200 credit for 30 days. **No perpetual free tier**. | **~$281B revenue (Microsoft FY2025)** |

| **[Amazon WorkSpaces](https://aws.amazon.com/workspaces/)** | **AWS-managed DaaS with persistent and non-persistent options.** WorkSpaces Personal for consistent desktops; WorkSpaces Pools for shared/intermittent use. | **Windows Value example**: **$25/month**; **Windows Standard example**: **$44/month** . AutoStop combines monthly base charge + hourly use. WorkSpaces Pools include instance + Windows access charges . | **AWS Free Tier**: $100–$200 credits for new accounts. **No perpetual free tier** for WorkSpaces. | **~$638B revenue (Amazon FY2025)** |

| **[Citrix DaaS](https://www.citrix.com/)** | **Enterprise-grade VDI and application delivery.** Virtual Apps and Desktops, hybrid deployment options, and mature policy/monitoring controls. | **Quote-based or calculator** — no public per-user rate . **Infrastructure and Microsoft licensing remain separate cost areas** . | **None** — enterprise demo required. | **Private (part of Cloud Software Group)** |

| **[Omnissa Horizon Cloud](https://www.omnissa.com/)** | **Enterprise VDI (formerly VMware Horizon).** Broad enterprise control, hybrid deployment, and mature management stack. | **Quote-based** — no public per-user rate . | **None** — enterprise demo required. | **Private (spun out of VMware/Broadcom)** |

| **[Dizzion Frame](https://www.dizzion.com/)** | **Cloud-native DaaS.** Multi-cloud support, browser-delivered desktops, and usage-based billing. | **Custom pricing** — quote required. | **Free trial** available on request. | **Private (~$50M+ raised)** |

| **[Kasm Cloud](https://kasm.com/)** | **Managed version of Kasm Workspaces.** Browser-delivered containers, applications, and desktops with SOC 2 Type II certification. | **Custom pricing** — quote required. Self-hosted Kasm Workspaces Community Edition is free . | **Free Community Edition** for self-hosting . **14-day trial** for Cloud. | **Private (Kasm Technologies)** |



## 🔓 Open-Source GitHub Projects



Sorted by star count (descending). Star badge links to each repo's stargazers page.



| Repo | Description | Stars |

|---|---|---|

| **[Apache Guacamole](https://github.com/apache/guacamole)** — **The de-facto clientless remote desktop gateway.** Supports **VNC, RDP, and SSH** through a web browser—no plugins or client software required . **1.6.0** (June 2025) added improved rendering performance, batch connection import, and Duo v4 support . **Apache-2.0**. | [![Stars](https://img.shields.io/github/stars/apache/guacamole?style=social&color=white)](https://github.com/apache/guacamole/stargazers) | ~3,500 |

| **[RustDesk](https://github.com/rustdesk/rustdesk)** — **Full-featured open-source remote control alternative.** Self-hosted with full data control. Supports Windows, macOS, Linux, iOS, Android, and Web. **VP8/VP9/AV1 software codecs + H264/H265 hardware codecs**. P2P connection with **NaCl end-to-end encryption** . **Self-host OSS Server** free, or **Pro Server** with web console, SSO, and enterprise controls . | [![Stars](https://img.shields.io/github/stars/rustdesk/rustdesk?style=social&color=white)](https://github.com/rustdesk/rustdesk/stargazers) | ~85,000 |

| **[IsardVDI](https://github.com/isard-vdi/isard)** — **Free Software desktop virtualization platform (AGPL v3).** KVM-based, **GPU support via NVIDIA Grid**, Docker/Docker Compose deployment in minutes, scalable multi-hypervisor management. Supports **SPICE, noVNC (web), RDP, and Guacamole RDP** viewers . | [![Stars](https://img.shields.io/github/stars/isard-vdi/isard?style=social&color=white)](https://github.com/isard-vdi/isard/stargazers) | ~51 |

| **[QVD (theqvd)](https://github.com/theqvd/theqvd)** — **Open Source VDI solution for Linux environments.** Provides a safe and easy-to-manage alternative to desktop and application virtualization . | [![Stars](https://img.shields.io/github/stars/theqvd/theqvd?style=social&color=white)](https://github.com/theqvd/theqvd/stargazers) | ~104 |



**Additional open-source options worth exploring:**



| Repo | Description |

|---|---|

| **[Apache CloudStack](https://github.com/apache/cloudstack)** — IaaS platform used for VDI deployments. **Eliminates hypervisor license costs**, reducing total cost per desktop for educational institutions . |

| **[Proxmox VE](https://github.com/proxmox/pve-manager)** — Open-source virtualization platform. **Kasm Workspaces integrates natively** with Proxmox VE API for auto-provisioning of worker VMs . |



## 🤝 How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## ⚠️ Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- DaaS platforms handle sensitive user data and corporate applications; ensure proper access controls, Zero Trust architecture, and compliance with organizational security policies.

- **Open-source reality**: The open-source ecosystem for DaaS is **mature and production-proven**. **Kasm Workspaces** delivers browser-based containers, applications, and desktops with **GPU acceleration, Zero Trust via OpenZiti, and native Proxmox VE integration** — trusted by **federal agencies for multi-segment secure network deployments** . **Apache Guacamole** is the de-facto clientless remote desktop gateway . **IsardVDI** provides a free KVM-based alternative with **GPU support** . **RustDesk** offers self-hosted remote control with **85,000+ stars** . However, **commercial platforms** (Citrix, Omnissa, Windows 365) provide **enterprise-grade management, compliance certifications, and dedicated support** that open-source alternatives require significant operational investment to match. The open-source path is **genuinely viable** for organizations with strong infrastructure engineering capacity.

- **Pricing caveat**: All pricing figures are **verified against cited search results** but may change without notice. **Windows 365** is priced per-user with fixed specs . **AWS WorkSpaces** pricing varies by region, bundle, storage, and OS . **Citrix and Omnissa** require formal quotes. Always request a formal quote for accurate budgeting.



---



**Made for IT administrators, VDI engineers, cloud architects, and infrastructure teams.**

Let's make Desktop-as-a-Service more open, transparent, and secure.
