---
title: "Κλάση License"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Aspose.Zip.License κλάση. Παρέχει μεθόδους για την άδεια του στοιχείου"
type: docs
weight: 660
url: /el/net/aspose.zip/license/
---
## License class

Παρέχει μεθόδους για την άδεια του στοιχείου.

```csharp
public sealed class License
```

## Κατασκευαστές

| Όνομα | Περιγραφή |
| --- | --- |
| [License](license/)() | Αρχικοποιεί μια νέα παρουσία της κλάσης `License`. |

## Μέθοδοι

| Όνομα | Περιγραφή |
| --- | --- |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense)(Stream) | Παρέχει άδεια στο στοιχείο. |
| [SetLicense](../../aspose.zip/license/setlicense/#setlicense_1)(string) | Παρέχει άδεια στο στοιχείο. |

## Παραδείγματα

Σε αυτό το παράδειγμα, θα γίνει προσπάθεια να βρεθεί ένα αρχείο άδειας με όνομα MyLicense.lic στον φάκελο που περιέχει το στοιχείο, στον φάκελο που περιέχει το καλούν σύνολο, στον φάκελο του συνόλου εισόδου και, τέλος, στους ενσωματωμένους πόρους του καλούντος συνόλου.

```csharp
[C#]

License license = new License();
license.SetLicense("MyLicense.lic");


[Visual Basic]

Dim license As license = New license
License.SetLicense("MyLicense.lic")
```

το αρχείο jar του στοιχείου:

```csharp
License license = new License();
license.setLicense("MyLicense.lic");
```

### Δείτε επίσης

* namespace [Aspose.Zip](../../aspose.zip/)
* assembly [Aspose.Zip](../../)


