---
title: Purchase Order Subscription
description: Wiederkehrende Bestellungen verwalten.
tags:
- HowTo
- Drittanbieter
prev: ./purchase
---
# Purchase Order Subscription
![icon_oms_box](attachments/icon_oms_box.png)

{{ $frontmatter.description }}

Technischer Name: `purchase_order_subscription`\
Repository: <https://github.com/Mint-System/Odoo-Apps-Purchase-Workflow/tree/16.0/purchase_order_subscription>

## Beschreibung

Mit dieser Erweiterung können Sie Bestellungen als Einkaufsabonnements konfigurieren. Odoo prüft täglich das Abrechnungsdatum der Einkaufsabonnements und erhöht die erhaltene Menge der Bestellzeilen und die bestellte Menge. Wenn Sie eine Lieferantenrechnung erfassen, können Sie das Einkaufsabonnment wieder auswählen.

## Verwendung

### Wiederkehrende Bestellung erfassen

Zeigen Sie eine Bestellung via *Einkauf* an oder erstellen Sie eine Neue. Im Feld *Wiederholung* wählen Sie den entsprechenden Intervall aus. Wenn Sie das Angebot bestätigen, erscheint das Feld *Nächstes Rechnungsdatum*.