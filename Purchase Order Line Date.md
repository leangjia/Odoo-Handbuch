---
title: Purchase Order Line Date
description: Lieferdatum im Wareneingang automatisch nachtragen.
tags:
- HowTo
- Drittanbieter
prev: ./purchase
---
# Purchase Order Line Date
![](attachments/icon_oms_box.png)

{{ $frontmatter.description }}

Technischer Name: `purchase_order_line_date`\
Repository: <https://github.com/Mint-System/Odoo-Apps-Purchase-Workflow/tree/16.0/purchase_order_line_date>

## Verwendung

### Lieferdatum aus Bestellung aktualisieren

Wenn Sie in der Positionszeile einer Bestellung das Lieferdatum aktualisieren, wird dieses im Wareneingang nachgetragen. Die Sicherheitsvorlaufzeit für den Einkauf wird wie folgt eingerechnet:

Geplantes Datum (Lagerbuchung) = Liefertermin (Bestellposition) + Sicherheitsvorlaufzeit Einkauf\
Frist (Lagerbuchung) = Liefertermin (Bestellposition)

Dazu ein Beispiel mit Sicherheitsvorlaufzeit von -3 Tagen.

![Purchase Order Line Date](attachments/Purchase%20Order%20Line%20Date.gif)