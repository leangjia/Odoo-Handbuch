---
title: Zeiterfassung Aktionen
description: Arbeitsflüsse in der Zeiterfassung automatisieren.
tags:
- HowTo
- Aktionen
prev: ./hr-timesheet
---
# Zeiterfassung Aktionen
![icons_odoo_hr_timesheet](attachments/icons_odoo_hr_timesheet.png)

## Aktionen

### Auftragselement von Aufgabe entfernen

*Gilt ab #Odoo14.*

Navigieren Sie nach *Einstellungen > Technisch > Server Aktionen* und erstellen Sie einen neuen Eintrag:

Name der Aktion: `Auftragselement von Aufgabe entfernen`\
Modell: `Kostenstellen-Buchungen`\
Folgeaktion: `Python-Code ausführen`

Kopieren Sie die folgenden Zeilen in das Feld Pythoncode:

```python
for record in records:
	record.task_id.write({'sale_line_id': False})
```

Die Aktion mit dem Knopf *Kontextuelle Aktion erstellen* bestätigen und dann speichern.

In der Ansicht von Kostenstellen-Buchungen erscheint nun in der Auswahl *Aktion* das Menu *Validierung zurücksetzen*.

### Validierung zurücksetzen

*Gilt ab #Odoo14.*

Navigieren Sie nach *Einstellungen > Technisch > Server Aktionen* und erstellen Sie einen neuen Eintrag:

Name der Aktion: `Validierung zurücksetzen`\
Modell: `Kostenstellen-Buchungen`\
Folgeaktion: `Python-Code ausführen`

Kopieren Sie die folgenden Zeilen in das Feld Pythoncode:

```python
for record in records:
	records.write({'validated': False})
```

Die Aktion mit dem Knopf *Kontextuelle Aktion erstellen* bestätigen und dann speichern.

In der Ansicht von Kostenstellen-Buchungen erscheint nun in der Auswahl *Aktion* das Menu *Validierung zurücksetzen*.