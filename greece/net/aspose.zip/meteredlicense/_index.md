---
title: "Κλάση MeteredLicense"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.MeteredLicense κλάση. Παρέχει μεθόδους για ορισμό κλειδιού με μέτρηση"
type: docs
weight: 760
url: /el/net/aspose.zip/meteredlicense/
---
## MeteredLicense class

Παρέχει μεθόδους για τον ορισμό κλειδιού μέτρησης.

```csharp
public class MeteredLicense
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [MeteredLicense](meteredlicense/)() | Ο προεπιλεγμένος κατασκευαστής. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [ResetMeteredKey](../../aspose.zip/meteredlicense/resetmeteredkey/)() | Αφαιρεί την προηγουμένως ρυθμισμένη άδεια. |
| [SetMeteredKey](../../aspose.zip/meteredlicense/setmeteredkey/)(string, string) | Ορίζει δημόσια και ιδιωτικά κλειδιά με μέτρηση. |
| static [GetConsumptionCredit](../../aspose.zip/meteredlicense/getconsumptioncredit/)() | Λαμβάνει πίστωση κατανάλωσης. |
| static [GetConsumptionQuantity](../../aspose.zip/meteredlicense/getconsumptionquantity/)() | Λαμβάνει το μέγεθος αρχείου κατανάλωσης. |

## Παραδείγματα

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να οριστούν δημόσιο και ιδιωτικό κλειδιά με μέτρηση

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

το αρχείο jar του στοιχείου:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

### Δείτε επίσης

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


