# ⚡ CyberSentinel — Cyber Threat Intelligence Command Center

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES2024-F7DF1E?style=for-the-badge&logo=javascript)
![Canvas API](https://img.shields.io/badge/Canvas_API-Real--Time-00C8FF?style=for-the-badge)
![Security](https://img.shields.io/badge/Cybersecurity-SOC%20Dashboard-ff2244?style=for-the-badge)
![Level](https://img.shields.io/badge/Master's-Research%20Project-9B59B6?style=for-the-badge)
![No Deps](https://img.shields.io/badge/Dependencies-ZERO-00ff88?style=for-the-badge)

> **CyberSentinel** is a full-featured, real-time Cyber Threat Intelligence Command Center built entirely in vanilla HTML/CSS/JavaScript with zero dependencies. It simulates a professional SOC (Security Operations Center) environment featuring a live global attack map, AI threat analyst, MITRE ATT&CK tracking, CVE monitoring, and animated threat intelligence feeds.

---

## 🎬 Live Preview

**[▶ Launch CyberSentinel](https://YOUR_USERNAME.github.io/cybersentinel)**

```
┌─────────────────────────────────────────────────────────────────┐
│  CYBERSENTINEL // THREAT INTELLIGENCE COMMAND CENTER    CRITICAL │
│  [ATTACKS/MIN: 1,847] [COUNTRIES: 49] [BLOCKED: 94,210]         │
├──────────────┬──────────────────────────────────┬───────────────┤
│ TOP ORIGINS  │                                  │ ACTIVE CVEs   │
│ 🇨🇳 China    │   [LIVE WORLD ATTACK MAP]        │ CVE-2024-3094 │
│ 🇷🇺 Russia   │   ╔══════════════════════╗       │ CVE-2024-1709 │
│ 🇺🇸 USA      │   ║ •→→→→→→→→→→→→→→• ●  ║       │ CVE-2024-4577 │
│ 🇧🇷 Brazil   │   ║  •→→→→• ●          ║       │               │
│              │   ╚══════════════════════╝       │ SENSOR NET    │
│ ATTACK TYPES │                                  │ HONEYPOT EU ✓ │
│ ████ DDoS    │  [ATTACKS] [HEAT] [ROUTES]       │ IDS CLUSTER ✓ │
│ ███  Ransom  │                                  │               │
│ ██   Phish   │                                  │ TRAFFIC CHART │
│              │                                  │ ╱╲  ╱╲╱╲╱╲   │
├──────────────┴─────────────────┬────────────────┴───────────────┤
│ LIVE THREAT FEED               │ ⬡ AI THREAT ANALYST            │
│ 14:22:31 [DDOS] China→Finance  │ ⚠ DDoS surge: financial sector │
│ 14:22:29 [RANS] Russia→Gov     │ ↑ 340% ransomware vs baseline  │
│ 14:22:27 [BRUT] DPRK→Energy    │ Attribution: Lazarus Group 87% │
└────────────────────────────────┴────────────────────────────────┘
```

---

## ✨ Features

### 🗺️ Live Global Threat Map
- Real-time animated attack arcs from source to target countries
- **3 view modes**: Attack arcs, Heat map overlay, Route visualization
- Hover tooltip showing attack type, source, and target
- Particle network background with connection visualization
- CRT scanline and vignette effects for authentic SOC aesthetic

### 📡 Live Intelligence Feed
- Scrolling real-time threat event stream
- Color-coded attack type badges (DDoS, Ransomware, Phishing, Brute Force, Exploit, Port Scan)
- Severity classification: CRITICAL / HIGH / MEDIUM
- Timestamped events with source country and target sector

### 🤖 AI Threat Analyst
- Simulated AI-powered threat commentary
- Attribution analysis (APT28, Lazarus Group, etc.)
- Anomaly detection alerts
- Actionable security recommendations

### 📊 Live Metrics Dashboard
- **Global threat counter** — live incrementing total
- **Attacks per minute** meter
- **Blocked threats percentage** — real-time bar
- **Network load, Firewall capacity, AI confidence** indicators
- **Malicious traffic chart** — animated time-series (Gbps)
- **Regional traffic breakdown** — EU, Americas, APAC, MENA

### 🔴 Threat Intelligence Panels
- **Top Attack Origins** — Top 10 countries with relative volume bars
- **Attack Vector Distribution** — Live donut chart with percentages
- **MITRE ATT&CK Framework** — Active technique tags (T1059–T1588)
- **Active CVE Monitor** — Live CVEs with CVSS scores
- **Sensor Network Status** — Honeypot and IDS cluster health

### 🎨 Design
- Full dark SOC aesthetic — deep navy/void palette with cyan glow accents
- Bebas Neue + JetBrains Mono + Exo 2 — carefully chosen type hierarchy
- CSS-only animations: pulse rings, feed transitions, AI typing indicator
- Canvas-rendered world map, donut chart, traffic chart, and sparkline
- Zero external dependencies — one HTML file, fully self-contained

---

## 🛠️ Installation

```bash
git clone https://github.com/YOUR_USERNAME/cybersentinel.git
cd cybersentinel
open index.html         # macOS
# OR
python -m http.server   # then visit localhost:8000
```

**Requirements:** Any modern browser. Zero dependencies. Zero setup.

---

## 🔬 Technical Architecture

```
CyberSentinel Architecture
│
├── Rendering Engine
│   ├── Canvas API — World map (land polygons, arcs, heat)
│   ├── Canvas API — Donut chart (attack vector distribution)
│   ├── Canvas API — Traffic time-series chart
│   ├── Canvas API — Sparkline (threat volume)
│   └── Canvas API — Particle network background
│
├── Simulation Engine
│   ├── Arc system — Bezier curve attack trajectories
│   ├── Heat map — Intensity accumulation per source
│   ├── Feed generator — Template-based event synthesis
│   └── AI message queue — Rotating analyst insights
│
├── State Management
│   ├── Attack statistics per vector type
│   ├── Traffic history (30-point rolling window)
│   ├── Threat counter with blocked percentage
│   └── Threat level classifier (LOW → CRITICAL)
│
└── UI Engine
    ├── CSS Grid — 3-column × 3-row responsive layout
    ├── CSS animations — Feed transitions, pulse rings, AI dots
    ├── Real-time DOM updates — 800ms master tick
    └── Mouse interaction — Hover tooltip on attack arcs
```

---

## 📚 Cybersecurity Concepts Demonstrated

| Concept | Implementation |
|---|---|
| **SOC Dashboard Design** | Full command center layout matching real SOC UIs |
| **MITRE ATT&CK Framework** | Active technique tags (T1566, T1190, T1486...) |
| **CVE Monitoring** | Real 2024 CVEs with accurate CVSS scores |
| **Threat Intelligence** | Attribution analysis, IOC tracking, TTPs |
| **Attack Taxonomy** | DDoS, Ransomware, Phishing, Brute Force, Exploit, Scan |
| **APT Groups** | Lazarus Group (DPRK), APT28 (Russia), references |
| **Geolocation Tracking** | Source-to-target attack routing by country |
| **Sensor Networks** | Honeypot + IDS cluster monitoring |

---

## 🔭 Future Roadmap

- [ ] Backend: Python Flask + WebSocket for real threat data
- [ ] Shodan API integration for live scanning activity
- [ ] AbuseIPDB API for real malicious IP lookups
- [ ] CISA KEV (Known Exploited Vulnerabilities) live feed
- [ ] AlienVault OTX threat feed integration
- [ ] Incident response playbook trigger system
- [ ] Multi-analyst collaboration mode
- [ ] SIEM alert escalation workflow

---

## 📄 License

MIT License — see LICENSE for details.

## ⚠️ Disclaimer

> This is a **simulation dashboard** for educational and demonstration purposes.  
> All threat data is procedurally generated. No real attack data is collected or displayed.  
> Built as part of a Master's-level Cybersecurity research portfolio.

---

## 👤 Author

**Master's Student — Cybersecurity**  
*"The best defense is understanding the offense."*
