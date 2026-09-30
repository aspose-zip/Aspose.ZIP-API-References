---
title: "MeteredLicense.SetMeteredKey"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Μέθοδος MeteredLicense. Ορίζει τα δημόσια και ιδιωτικά κλειδιά μετρητή"
type: docs
weight: 30
url: /el/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Ορίζει δημόσια και ιδιωτικά κλειδιά με μέτρηση.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| publicKey | String | Το δημόσιο κλειδί. |
| privateKey | String | Το ιδιωτικό κλειδί. |

## Παρατηρήσεις

Εάν αγοράσετε μια metered license, αυτό το API πρέπει να κληθεί κατά την εκκίνηση της εφαρμογής· συνήθως αυτό είναι αρκετό. Ωστόσο, εάν η metered αποτύχει να ανεβάσει τα δεδομένα κατανάλωσης κατά τη διάρκεια μιας περιόδου 24 ωρών, η άδεια θα οριστεί σε κατάσταση αξιολόγησης. Για να αποφύγετε αυτή την περίπτωση, θα πρέπει να ελέγχετε τακτικά την κατάσταση της άδειας. Εάν είναι σε κατάσταση αξιολόγησης, καλέστε ξανά αυτό το API.

### Δείτε επίσης

* class [MeteredLicense](../)
* namespace [Aspose.Zip](../../meteredlicense/)
* assembly [Aspose.Zip](../../../)


