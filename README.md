# 🛡️ Windows Server GRC Lab

## 🎯 Ziel des Projekts

Dieses Projekt simuliert eine Unternehmensumgebung zur praktischen Umsetzung von IT-Audits und GRC-Maßnahmen (Governance, Risk, Compliance).  
Ziel ist es, mit **Windows Server 2022** ein Active Directory (AD), Gruppenrichtlinien (GPOs), Benutzer- und Zugriffsmanagement sowie Sicherheitsrichtlinien aufzubauen und diese gemäß folgenden Standards zu prüfen:

- ✅ **ISO/IEC 27001:2022**
- ✅ **BSI IT-Grundschutz**
- ✅ **DSGVO (Datenschutz-Grundverordnung)**
- ✅ **NIST Cybersecurity Framework**

---

## 🗂️ Projektstruktur


windows-server-grc-lab/
│
├── 📁 Dokumentation/       # PDF-Berichte, Audit-Protokolle, Richtlinien
├── 📁 Screenshots/         # Visuelle Nachweise (Benutzer, GPOs, AD-Struktur)
├── 📁 Skripte/             # PowerShell-Skripte, Setup-Skripte
├── 📁 Policies/            # GPO-Exporte, Passwort-Richtlinien, ISO-Mappings
└── 📄 README.md            # Diese Projektbeschreibung


## 🧰 Verwendete Tools & Technologien

- 🪟 **Windows Server 2022**
- 🧩 **Active Directory Domain Services (AD DS)**
- ⚙️ **Group Policy Management (GPMC)**
- 🔐 **Lokale Sicherheitsrichtlinien**
- 🧾 **ISO/IEC 27001 Kontrollen**
- 🛡️ **DSGVO Technisch-organisatorische Maßnahmen (TOMs)**
- 📸 **Screenshots zur Nachweisführung**



## 🛠️ Umsetzungsschritte (Beispiel)

1. **AD-Domäne einrichten** (`dc01.christian.grc.local`)
2. **Organisationseinheiten (OUs) anlegen** für Abteilungen
3. **Benutzerkonten und Gruppen** in AD anlegen
4. **Passwortrichtlinie via GPO konfigurieren**
5. **Sicherheitsrichtlinien mappen** auf ISO 27001 / BSI / DSGVO
6. **Dokumentation & Screenshots** sichern
7. **Audit-Protokolle erstellen** (z. B. mit Checklisten)




## 📚 Lernziele / Nutzen

- Praxisnahe Umsetzung von IT-GRC-Audits
- Vorbereitung auf ISO 27001 Audits / BSI Grundschutz Assessments
- GitHub-Projekt als Nachweis für Vorstellungsgespräche in Deutschland
- Verbesserung von technischem Vokabular auf Deutsch



## 🧑‍💻 Autor

**Christian Chukwuka**  
Zertifiziert in CISA, CISM, ISO 27001 Lead Auditor  
MSc in Data Analytics, HDip Cybersecurity GRC  
📍 Deutschland


