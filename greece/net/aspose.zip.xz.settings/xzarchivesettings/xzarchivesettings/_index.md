---
title: "XzArchiveSettings.XzArchiveSettings"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής XzArchiveSettings. Αρχικοποιεί μια νέα παρουσία της κλάσης XzArchiveSettings χρησιμοποιώντας μονή συμπίεση LZMA2."
type: docs
weight: 10
url: /el/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XzArchiveSettings`](../) χρησιμοποιώντας μονή συμπίεση LZMA2.

```csharp
public XzArchiveSettings()
```

## Παρατηρήσεις

Το προεπιλεγμένο λεξικό στο φίλτρο LZMA2 έχει μέγεθος 16 megabytes, το προεπιλεγμένο μέγεθος μπλοκ είναι 64 megabytes, ο προεπιλεγμένος τύπος αθροίσματος ελέγχου είναι CRC32.

### Δείτε επίσης

* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`XzArchiveSettings`](../) με προσαρμοσμένες παραμέτρους.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filters | XzFilterSettings[] | Φίλτρα (συμπιεστές) που θα εφαρμοστούν διαδοχικά για τη δημιουργία του [`XzArchive`](../../../aspose.zip.xz/xzarchive/). Μπορεί να είναι είτε ένα μόνο [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) είτε ένα ζεύγος των [`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) και [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |
| blockSize | Int64 | Μέγεθος μπλοκ xz αρχείου. |
| checkType | XzCheckType | Τύπος υπολογισμού αθροίσματος ελέγχου για ασυμπίεστα δεδομένα. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* είναι αρνητικό. |
| ArgumentNullException | *filters* είναι null |
| ArgumentException | *filters* έχει λιγότερο από ένα ή περισσότερα από δύο φίλτρα, ή το τελευταίο φίλτρο δεν είναι [`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

## Παραδείγματα

```csharp
using (FileStream xzFile = File.Open("archive.xz", FileMode.Create))
{
    XzLZMA2FilterSettings filter = new XzLZMA2FilterSettings(5242880);
    XzArchiveSettings settings = new XzArchiveSettings(new XzFilterSettings[] {filter}, 10485760, XzCheckType.Crc32);
    using (var archive = new XzArchive(settings))
    {
        archive.SetSource("data.bin");
        archive.Save(xzFile);
     }
}
```

### Δείτε επίσης

* class [XzFilterSettings](../../xzfiltersettings/)
* enum [XzCheckType](../../xzchecktype/)
* class [XzArchiveSettings](../)
* namespace [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* assembly [Aspose.Zip](../../../)


