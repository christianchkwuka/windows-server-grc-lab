Windows Server GRC Lab – Domänencontroller- 
Konfiguration (ISO 27001, BSI, DSGVO, NIST) 
1.	Zielsetzung 
Einrichtung eines Domänencontrollers mit Active Directory, DNS und GPOs zur Simulation eines GRC-AuditSzenarios. 
  
2.	Server-Vorbereitung (Windows Server 2022) 
 Einstellungen in VirtualBox: 
•	RAM: mindestens 7040 MB (7 GB) 
•	Prozessoren: 4 
•	Netzwerk: NAT oder Bridged Adapter (mit Internetzugang) 
  
3.	Netzwerkkonfiguration (statische IP) 
1. Rechtsklick auf Netzwerk > Eigenschaften > IPv4 konfigurieren 2. Beispiel: 
3.	IP-Adresse: 192.168.1.10 
4.	Subnetzmaske: 255.255.255.0 
5.	Gateway: 192.168.1.1 
6.	DNS: 192.168.1.10 (wenn lokal) 
  
4.	Windows Server auf Deutsch umstellen (optional) 
1.	Systemsteuerung > Sprache 
2.	Deutsch (Deutschland) hinzufügen 
3.	Als Anzeigesprache festlegen & Neustart 
  
5.	Rollen & Features installieren 
 Schritte: 
1.	Start > Server-Manager > Verwalten > Rollen und Features hinzufügen 
2.	Installationstyp: Rollenbasierte oder featurebasierte Installation 3. Zielserver: Lokaler Server auswählen 
4.	Serverrollen: 
5.	[x] Active Directory Domain Services 
6.	[x] DNS-Server 
1 
7.	[x] Dateidienste (optional) 
8.	Features: Voreinstellungen übernehmen 
9.	Installation abschließen 
  
6.	Domänencontroller einrichten 
 Bereitstellung einer neuen Gesamtstruktur 
1.	Nach Installation erscheint Hinweis im Server-Manager: "Server zu einem Domänencontroller heraufstufen" 
2.	Bereitstellungskonfiguration: Neue Gesamtstruktur hinzufügen 3. Stammdomäne: z. B. intern.local 
4.	Domänencontrolleroptionen: 
5.	Funktionsebene: Windows Server 2016 oder höher 
6.	DNS-Server aktivieren 
7.	Kennwort für Verzeichnisdienste-Wiederherstellungsmodus (DSRM) festlegen 
8.	DNS-Warnung ignorieren (wenn ohne Weiterleitung) 
9.	NetBIOS-Domänenname bestätigen (automatisch) 
10.	Pfade lassen (Standard) 
11.	Zusammenfassung prüfen & Installation starten 
12.	Neustart nach Abschluss 
  
7.	Firewall prüfen 
1.	Öffne die Firewall-Einstellungen: 
2.	Start > wf.msc 
3.	Überprüfe eingehende Regeln: 
4.	Remote Desktop (Port TCP 3389) – erlaubt 
5.	Ping (ICMP Echo-Anfrage) – erlaubt 
  
8.	Test und Neustart 
1.	Server neu starten 
2.	Remote Desktop Verbindung testen 
3.	Mit IP-Adresse verbinden: z. B. 192.168.1.10 
4.	Erreichbarkeit dokumentieren 
5.	Screenshot: Netzwerkinfo + IP-Adresse 
6.	Notiz: Ping & RDP erreichbar (Ja/Nein) 
  

