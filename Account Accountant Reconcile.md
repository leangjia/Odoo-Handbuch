---
title: Account Accountant Reconcile
description: Bank-Gutschriften anhand Referenz und Betrag abgleichen.
tags:
- HowTo
- Drittanbieter
prev: ./accounting
---
# Account Accountant Reconcile
![icon_oms_box](attachments/icon_oms_box.png)

{{ $frontmatter.description }}

Technischer Name: `account_acountant_reconcile`\
Repository: <https://github.com/Mint-System/Odoo-Apps-Account-Reconcile/tree/16.0/account_acountant_reconcile>

## Beschreibung

Beim Import von Kontoauszügen versucht Odoo die Kontoauszugszeilen automatisch abzustimmen. Diese Erweiterung ersetzt die bestehende Abstimmungs-Methode. Sie sucht die passende Rechnungszeilen anhand der Zahlungsreferenz und des Betrags und gleicht diese bei einer eindeutigen Übereinstimmung ab. 

## Verwendung

### Automatische Abstimmung manuell ausführen

Navigieren Sie nach *Einstellungen > Technisch > Geplante Aktionen* und rufen Sie die Aktion *Versuchen Sie, Ihre Kontoauszugszeilen automatisch abzustimmen* auf. Führen Sie diese Aktion mit *Manuell Ausführen* aus.