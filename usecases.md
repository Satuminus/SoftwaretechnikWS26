# 1 Fachliche Grundlagen und Anforderungen (Team A)

## 1.1 Produktvision
### 1.1.1 Zielsetzung des Softwareprodukts
Die Zielsetzung des Softwareprodukts ist es, eine Zentrale Platform zur Planung, Organisation, Durchführung und Nachbereitung von Veranstaltungen zu erstellen. Dazu sollen viele verschiedene Tools zusammengelegt werden, wie zum Beispiel verschiedene Messenger, Email, Excel und Ticketsysteme. Also sammelt man alle relevanten Informationen an einem Ort/ auf einer Platform. Das System soll Transparenz über Termine, Aufgaben, Finanzen und Teilnehmer bieten. Dabei soll das Softwareprodukt sowohl für private als auch kommerziele Nutzung dienen. Weitere Anforderungen sind die Endgeräteunabhänigkeit und die Skalierbarkeit des Produktes. Das Produkt bietet eine Kombination aus Eventplanung, Finanzverwaltung und Dienstleisterintegration.
### 1.1.2 Produktname und Begründung
Wir nennen das Softwareprodukt "EventHub". Der Name ist leicht merkbar und simpel, spiegelt den Zweck der Software gut wieder und international verständlich. Außerdem ist er nicht zu technisch aber gleichzeitig professionell.

## 1.2 Akteure und Rollen
### 1.2.1 Nicht registrierte/unangemeldete Akteure
Ein nicht angemeldeter Akteuer hat folgende Optionen:
- Registrierung durchführen
- Login durchführen
- öffentliche Event- und Dienstleisterseiten aufrufen
### 1.2.2 Registrierte Akteuere
#### 1.2.2.1 Privatnutzer/Teinehmer
Das sind die Nutzer, die Events beitreten und dran teilnehmen. Sie können:
- sich registrieren/anmelden
- Gruppen beitreten/verlassen
- Notizen, Termine, Umfragen erstellen und dran teilnehmen
- abstimmen & kommentieren
- Einzahlungen vornehmen
- Aufgaben übernehmen
- Medien hochladen
- Kalender synchronisieren
#### 1.2.2.3 Gruppenmitglied
Ein Gruppenmitglied kann:
- Inhalte einer Gruppe lesen
- Notizen erstellen/bearbeiten/löschen
- an Umfragen teilnehmen
- Aufgaben übernehmen
- Einzahlungen vornehmen
- Multimedia hochladen
- Gruppe verlassen

#### 1.2.2.4 Organisator/Gruppenleiter
- Gruppe/Event erstelllen und löschen
- Mitglieder einladen/entfernen/sperren
- Beitrittscode verwalten
- Mindestteilnehmerzahl festlegen
- Mindestbudget festlegen
- Aufgaben zuweisen
- Rückzahlungen veranlassen
- Eventseite verwalten
- Übersicht über Finanzen
- Moderationsmöglichkeiten

#### 1.2.2.5 Insitutionsadministrator
Das können zum Beispiel Lehrer oder Firmenverantwortliche sein:
- meherer Events verwalten
- Rollen und Berechtigungen vergeben
- Benutzerkonten innerhalb der Institution verwalten
- Übersicht über alle Veranstaltungen der Organisation
- Nutzungslimits überwachen
- Abrechnungen/Events archivieren

#### 1.2.2.6 Instituitionsmitglied
- meist nur leserechte
- Teilnahme an Events
- Aufgaben ausführen

#### 1.2.2.7 Veranstaltungs-Dienstleister
- eigenes Profil/Homepage verwalten
- Eventanfragen empfangen
- Angebote erstellen
- Rechnungen generieren
- Ressourcen planen
- Material und Personal verwalten
- Budgets kalkulieren
- durch Kunden bewerten lassen

#### 1.2.2.8 Mitarbeiter eines Dienstleisters
- persönliche Verfügbarkeit pflegen
- Einsätze/Arbeitspläne einsehen
- Benachrichtigungen bei Zuweisung erhalten
- Qualifikationen verwalten

#### 1.2.2.9 Kunde/Veranstalter (extern)
- Event anfragen
- Budget angeben
- Angebote erhalten
- Angebote annehmen und ablehnen
- Rechnungen bezahlen
- Dienstleister bewerten
### 1.2.3 Sekundäre Akteuere

#### 1.2.3.1 Externe Systeme
- Kalenderdienste (z.B Outlook, Google Kalender)
- Kommunikationsdienste (E-Mail, SMS, Messenger)
- Zahlungsdienste
- Ticketing-Systeme
- Datenaustausch über APIs

#### 1.2.3.2 Systemadministator
- Benutzer sperren/verwalten
- Systemkonfiguration
- Backups/Wartung

#### 

## 1.3 Glossar der Fachdomäne
### 1.3.1 Begriffsdefinitionen


# 2 Funktionale Anforderungen

## 2.1 Funktionale Gruppen Übersicht

- FG1 Account und Authentifizierung
- FG2 Profil und Einstellungen
- FG3 Gruppen- und Eventmanagement
- FG4 Notizen und Umfragen
- FG5 Finanzen
- FG6 Aufgabenmanagement
- FG7 Medien und Dokumentation
- FG8 Rollen- und Rechtesystem
- FG9 Öffentliche Eventseite und QR-Code
- FG10 Integration und Benachrichtigungen
- FG11 Dienstleister und Anfragen
- FG12 Angebote, Rechnungen und Mahnungen
- FG13 Ressourcenplanung

## 2.2 FG1 Account und Authentifizierung

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-01 Registrierung | Gast | mich registrieren | ich das System nutzen kann | Pflichtfelder sind ausgefüllt und Account wird erstellt | Muss |
| US-02 Login | Benutzer | mich anmelden | ich Zugriff auf meine Daten habe | korrekte Zugangsdaten erlauben Anmeldung | Muss |
| US-03 Logout | Benutzer | mich abmelden | niemand mein Konto missbraucht | Sitzung wird beendet | Muss |
| US-04 Passwort zurücksetzen | Benutzer | mein Passwort zurücksetzen | ich wieder Zugriff bekomme | Reset-Link oder Code ermöglicht neues Passwort | Muss |
| US-05 2FA aktivieren | Benutzer | Zwei-Faktor-Authentifizierung nutzen | mein Account sicherer ist | zusätzlicher Faktor wird beim Login geprüft | Sollte |

## 2.3 FG2 Profil und Einstellungen

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-06 Profil anzeigen | Benutzer | mein Profil sehen | ich meine Daten prüfen kann | gespeicherte Daten werden angezeigt | Muss |
| US-07 Profil bearbeiten | Benutzer | meine Daten ändern | sie aktuell bleiben | Änderungen werden gespeichert | Muss |
| US-08 Kommunikationsweg wählen | Benutzer | bevorzugte Benachrichtigungen einstellen | ich passende Nachrichten erhalte | gewählter Kanal wird gespeichert | Sollte |
| US-09 Sprache wählen | Benutzer | die Sprache ändern | ich die Oberfläche verstehe | UI-Texte werden angepasst | Sollte |

## 2.4 FG3 Gruppen- und Eventmanagement

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-10 Gruppe erstellen | Organisator | eine Gruppe anlegen | ich ein Event planen kann | Name und Beschreibung werden gespeichert | Muss |
| US-11 Gruppe löschen | Organisator | meine Gruppe löschen | alte Events entfernt werden | Gruppe wird archiviert oder gelöscht | Muss |
| US-12 Gruppe beitreten | Benutzer | einer Gruppe beitreten | ich teilnehmen kann | gültiger Beitrittscode erlaubt Beitritt | Muss |
| US-13 Gruppe verlassen | Benutzer | eine Gruppe verlassen | ich nicht mehr beteiligt bin | Mitgliedschaft endet | Muss |
| US-14 Mitglieder anzeigen | Benutzer | alle Mitglieder sehen | ich Überblick habe | Liste wird angezeigt | Muss |
| US-15 Mitglieder verwalten | Organisator | Mitglieder entfernen oder sperren | Regeln durchgesetzt werden | Zugriff wird entzogen | Muss |
| US-16 Mindestteilnehmer festlegen | Organisator | eine Mindestzahl definieren | Event nur bei genug Teilnehmern stattfindet | Status wird automatisch geprüft | Sollte |

## 2.5 FG4 Notizen und Umfragen

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-17 Notiz erstellen | Benutzer | eine Notiz anlegen | Infos dokumentiert sind | Notiz erscheint in der Liste | Muss |
| US-18 Notiz bearbeiten | Benutzer | Notizen ändern | Fehler korrigiert werden | Änderungen werden gespeichert | Muss |
| US-19 Notiz löschen | Benutzer | Notizen entfernen | irrelevante Infos verschwinden | Notiz wird entfernt | Muss |
| US-20 Notizen filtern | Benutzer | nach Typ filtern | ich schneller finde, was ich suche | Filter zeigt passende Einträge | Sollte |
| US-21 Termin erfassen | Benutzer | Termine mit Datum und Ort speichern | alle informiert sind | Termin enthält strukturierte Felder | Muss |
| US-22 Umfrage erstellen | Benutzer | eine Umfrage anlegen | Entscheidungen getroffen werden | Antwortoptionen frei wählbar | Muss |
| US-23 Abstimmen | Benutzer | an Umfragen teilnehmen | meine Meinung zählt | Stimme wird gezählt | Muss |
| US-24 Ergebnis anzeigen | Benutzer | Ergebnisse sehen | Transparenz besteht | Stimmenverteilung wird angezeigt | Muss |

## 2.6 FG5 Finanzen

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-25 Einzahlung tätigen | Benutzer | Geld einzahlen | Event finanziert wird | Betrag wird gespeichert | Muss |
| US-26 Zahlungsstand anzeigen | Benutzer | Gesamtbetrag sehen | ich Überblick habe | eingegangenes Geld und Zielsumme werden angezeigt | Muss |
| US-27 Ausgabe erfassen | Benutzer | Ausgaben dokumentieren | Kosten transparent sind | Betrag und Beschreibung werden gespeichert | Muss |
| US-28 Kassenübersicht | Organisator | alle Einnahmen und Ausgaben sehen | ich abrechnen kann | Summen werden korrekt berechnet | Muss |
| US-29 Rückzahlung auslösen | Organisator | Rückzahlungen durchführen | Guthaben ausgeglichen wird | Rückzahlung wird dokumentiert | Sollte |

## 2.7 FG6 Aufgabenmanagement

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-30 Aufgabe erstellen | Organisator | Aufgaben anlegen | To-dos geplant sind | Aufgabe erscheint in Liste | Muss |
| US-31 Aufgabe übernehmen | Benutzer | Aufgaben übernehmen | Zuständigkeit klar ist | Aufgabe wird mir zugeordnet | Muss |
| US-32 Aufgabe abschließen | Benutzer | Aufgaben als erledigt markieren | Fortschritt sichtbar ist | Status ändert sich auf erledigt | Muss |
| US-33 Erinnerung senden | System | an offene Aufgaben erinnern | nichts vergessen wird | Benachrichtigung wird automatisch gesendet | Sollte |

## 2.8 FG7 Medien und Dokumentation

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-34 Medien hochladen | Benutzer | Fotos oder Videos hochladen | das Event dokumentiert ist | Dateien werden gespeichert und angezeigt | Sollte |
| US-35 Kommentare schreiben | Benutzer | Bewertungen oder Kommentare hinterlassen | Erfahrungen geteilt werden | Text wird gespeichert | Könnte |

## 2.9 FG8 Rollen- und Rechtesystem

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-36 Rollen vergeben | Institutionsadmin | Rollen zuweisen | Rechte gesteuert werden | Berechtigungen werden gespeichert | Muss |
| US-37 Leserechte einschränken | Institutionsmitglied | nur lesen können | Regeln eingehalten werden | Schreibfunktionen deaktiviert | Muss |
| US-38 Lizenzlimit prüfen | Institutionsadmin | Events begrenzen | Community-Regeln gelten | mehr als drei Events werden verhindert | Sollte |

## 2.10 FG9 Öffentliche Eventseite und QR-Code

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-39 Eventseite anzeigen | Organisator | eine öffentliche Seite haben | ich das Event bewerben kann | feste URL ist erreichbar | Sollte |
| US-40 QR-Code generieren | Benutzer | einen QR-Code erhalten | ich den Link schnell teilen kann | Code wird korrekt erzeugt | Sollte |

## 2.11 FG10 Integration und Benachrichtigungen

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-41 Kalender synchronisieren | Benutzer | Termine synchronisieren | sie automatisch im Kalender erscheinen | Synchronisation funktioniert | Könnte |
| US-42 Benachrichtigungen senden | System | Nachrichten versenden | Nutzer informiert bleiben | Versand über gewählten Kanal erfolgt | Sollte |

## 2.12 FG11 Dienstleister und Anfragen

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-43 Anfrage stellen | Kunde | ein Event anfragen | ich ein Angebot erhalte | Formular speichert alle Pflichtdaten | Muss |
| US-44 Angebot erstellen | Dienstleister | ein Angebot generieren | ich Kunden informieren kann | Angebotsdokument wird erstellt | Muss |
| US-45 Rechnung erstellen | Dienstleister | eine Rechnung erzeugen | ich abrechnen kann | Rechnung enthält alle Pflichtangaben | Muss |
| US-46 Zahlung erinnern | System | an offene Rechnungen erinnern | Zahlungen rechtzeitig eingehen | Erinnerung wird automatisch versendet | Sollte |

## 2.13 FG12 Ressourcenplanung

| Name/ID | In meiner Rolle als... | ...möchte ich... | ..., so dass... | Akzeptiert, wenn... | Priorität |
|----------|----------------------|-----------------|----------------|--------------------|-----------|
| US-47 Material verwalten | Dienstleister | Material anlegen oder ändern | Bestand aktuell bleibt | Materialdaten werden gespeichert | Muss |
| US-48 Material buchen | Dienstleister | Material einem Event zuordnen | Doppelbuchungen vermieden werden | Material ist im Zeitraum gesperrt | Muss |
| US-49 Mitarbeiter verwalten | Dienstleister | Mitarbeiter planen | Personal verfügbar ist | Einsatzplan berücksichtigt Verfügbarkeit | Muss |
| US-50 Wartungshinweis | System | Wartungen anzeigen | Geräte sicher bleiben | Hinweis erscheint bei fälligem Zyklus | Sollte |


# 3 Nicht-funktionale Anforderungen (ISO 25010)

## 3.1 Usability
## 3.2 Performance und Skalierbarkeit
## 3.3 Sicherheit
## 3.4 Datenschutz (DSGVO)
## 3.5 Zuverlässigkeit und Verfügbarkeit
## 3.6 Kompatibilität (Browser, Mobile, Plattformen)
## 3.7 Wartbarkeit und Erweiterbarkeit
## 3.8 Barrierefreiheit und Internationalisierung

# 4 Graphische Benutzungsschnittstelle

## 4.1 Designprinzipien und UX-Grundlagen

## 4.2 Navigationsmodelle
### 4.2.1 Zustandsdiagramm – Privatnutzer
### 4.2.2 Zustandsdiagramm – Organisator
### 4.2.3 Zustandsdiagramm – Dienstleister

## 4.3 Webbrowser-Mockups
### 4.3.1 Login & Registrierung
### 4.3.2 Dashboard
### 4.3.3 Gruppenübersicht
### 4.3.4 Event-Detailseite
### 4.3.5 Finanzen
### 4.3.6 Notizen & Umfragen
### 4.3.7 Aufgabenplanung
### 4.3.8 Profil & Einstellungen

## 4.4 Mobile-App-Mockups
### 4.4.1 Navigation und Besonderheiten
### 4.4.2 Screens analog zur Webversion

## 4.5 Zuordnung Screens ↔ User Stories
