# 🖥️ Command Center Pro

> Windows-Tool zum Verwalten und blitzschnellen Ausführen von Systembefehlen — kein PowerShell-Fenster, kein Aufwand.

Entwickelt von **[SBS-ug.de](https://sbs-ug.de)**

---

## ✨ Features

- **Ein Klick = Befehl ausführen** — direkt oder im CMD-Fenster
- **CMD-Modus** — Ausgabe bleibt 15 Sekunden sichtbar, Fenster schließt automatisch
- **Befehle verwalten** — hinzufügen, bearbeiten und löschen per Rechtsklick-Menü
- **Suche** — Befehle in Echtzeit filtern
- **JSON-Konfiguration** — `commands.json` liegt neben der EXE, portabel und editierbar
- **Kein PowerShell-Fenster** — startet vollständig unsichtbar im Hintergrund
- **CMD-Badge** — visueller Hinweis welche Befehle im CMD-Fenster laufen

---

## 📦 Installation

1. `CommandCenterPro.exe` herunterladen
2. Doppelklicken
3. Fertig — kein Installer, keine Abhängigkeiten

> Beim ersten Start wird `commands.json` automatisch neben der EXE erstellt.

---

## 🚀 Verwendung

| Aktion | Beschreibung |
|---|---|
| **Linksklick** auf einen Befehl | Befehl ausführen |
| **Rechtsklick** auf einen Befehl | Bearbeiten oder Löschen |
| **+ Neu** | Neuen Befehl hinzufügen |
| **Suchfeld** | Befehle nach Name oder Befehlstext filtern |

### Befehl hinzufügen

1. Auf **+ Neu** klicken
2. Name und Befehl eingeben
3. Optional: *„Im CMD-Fenster ausführen"* aktivieren (empfohlen für `ping`, `ipconfig`, etc.)
4. **Speichern**

---

## ⚙️ commands.json

Befehle werden in einer einfachen JSON-Datei gespeichert und können auch direkt bearbeitet werden:

```json
{
  "buttons": [
    {
      "name": "IP-Adresse anzeigen",
      "command": "ipconfig /all",
      "cmdWindow": true
    },
    {
      "name": "Notepad öffnen",
      "command": "notepad.exe",
      "cmdWindow": false
    }
  ]
}
```

| Feld | Typ | Beschreibung |
|---|---|---|
| `name` | String | Anzeigename des Buttons |
| `command` | String | Auszuführender Befehl oder Programmpfad |
| `cmdWindow` | Boolean | `true` = CMD-Fenster öffnen, `false` = silent |

---

## 🛠️ Technische Details

- **Plattform:** Windows 10 / 11
- **Voraussetzung:** PowerShell 5.1+ (ab Windows 10 vorinstalliert)
- **Portabel** — läuft direkt vom USB-Stick oder Netzlaufwerk
- **Keine Admin-Rechte** für die App selbst erforderlich

---

## 📄 Lizenz

MIT License — freie Verwendung, auch kommerziell.

---

<div align="center">

Entwickelt mit ❤️ von **[SBS-ug.de](https://sbs-ug.de)**

</div>
