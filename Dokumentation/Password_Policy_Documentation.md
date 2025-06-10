# 🛡️ Kennwortrichtlinie / Password Policy

## 🎯 Ziel / Objective
Diese Richtlinie stellt sicher, dass Benutzer sichere Passwörter verwenden, um unbefugten Zugriff zu verhindern.  
This policy ensures that users use strong passwords to prevent unauthorized access.

## 📂 GPO-Name / GPO Name
**Kennwortrichtlinie_IT / PasswordPolicy_IT**

## 📍 Pfad / Path
Computerkonfiguration > Richtlinien > Windows-Einstellungen > Sicherheitseinstellungen > Kontorichtlinien > Kennwortrichtlinie  
Computer Configuration > Policies > Windows Settings > Security Settings > Account Policies > Password Policy

## ⚙️ Einstellungen / Settings
| Einstellung (DE)                            | Setting (EN)                          | Wert / Value      |
|--------------------------------------------|---------------------------------------|-------------------|
| Minimale Kennwortlänge                     | Minimum password length               | 12 Zeichen        |
| Kennwortkomplexität erzwingen              | Enforce password complexity           | Aktiviert / Enabled |
| Maximale Kennwortgültigkeit                | Maximum password age                  | 30 Tage / Days    |
| Alte Kennwörter merken (Verlauf)           | Remember password history             | 24 Kennwörter     |
| Mindestkennwortalter                       | Minimum password age                  | 1 Tag / Day       |

## 🧠 Begründung / Justification
Sichere Kennwörter schützen vor Brute-Force- und Wörterbuchangriffen.  
Strong passwords protect against brute-force and dictionary attacks.

## 🧪 Validierung / Validation
- `gpresult /r` Ausgabe zur Bestätigung der aktiven GPO  
- Screenshot der GPO-Einstellungen in GPMC  
- Passwort-Test mit schwachem Passwort, z. B. „1234“ → Fehlermeldung

## 🧾 Compliance Mapping
| Kontrolle / Control               | Standard           | Nachweis / Evidence                      |
|----------------------------------|--------------------|------------------------------------------|
| Benutzerregistrierung (A.9.2.1)  | ISO 27001:2022     | GPO + Screenshot                         |
| Passwortkomplexität (OPS.1.1.1)  | BSI Grundschutz    | `net accounts` + `gpresult /r`           |
| Sicherheit der Verarbeitung      | DSGVO Art. 32      | Screenshots + Ereignisprotokolle / logs  |

## 🛠 Tools & Commands
- GPMC (Group Policy Management Console)
- `gpresult /r`
- `net accounts`
- Event Viewer

## 📸 Screenshots (Empfohlen)
- Screenshots/Kennwortrichtlinie_GPMC.png
- Screenshots/gpresult_password_policy.png
- Screenshots/test_password_rejection.png

---
**Status:** ✅ Abgeschlossen / Completed  
**Autor:** Christian Chukwuka  
**Datum:** 2025-06-09