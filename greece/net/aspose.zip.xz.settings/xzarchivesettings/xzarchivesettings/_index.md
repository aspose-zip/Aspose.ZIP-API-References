---
title: XzArchiveSettings.XzArchiveSettings
second_title: Aspose.ZIP για Αναφορά API .NET
description: XzArchiveSettings κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουXzArchiveSettings κλάση με χρήση απλής συμπίεσης LZMA2.
type: docs
weight: 10
url: /el/net/aspose.zip.xz.settings/xzarchivesettings/xzarchivesettings/
---
## XzArchiveSettings() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`XzArchiveSettings`](../) κλάση με χρήση απλής συμπίεσης LZMA2.

```csharp
public XzArchiveSettings()
```

### Παρατηρήσεις

Το προεπιλεγμένο λεξικό στο μέγεθος φίλτρου LZMA2 ισούται με 16 megabyte, το προεπιλεγμένο μέγεθος μπλοκ ισούται με 64 megabyte, ο προεπιλεγμένος τύπος αθροίσματος ελέγχου είναι CRC32.

### Δείτε επίσης

* class [XzArchiveSettings](../)
* χώρος ονομάτων [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* συνέλευση [Aspose.Zip](../../../)

---

## XzArchiveSettings(XzFilterSettings[], long, XzCheckType) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`XzArchiveSettings`](../) κλάση με προσαρμοσμένες παραμέτρους.

```csharp
public XzArchiveSettings(XzFilterSettings[] filters, long blockSize, XzCheckType checkType)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| filters | XzFilterSettings[] | Φίλτρα (συμπιεστές) που θα εφαρμοστούν διαδοχικά για τη δημιουργία[`XzArchive`](../../../aspose.zip.xz/xzarchive/) . Μπορεί να είναι είτε single[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) ή ζεύγος[`XzBcjX86FilterSettings`](../../xzbcjx86filtersettings/) και[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/) |
| blockSize | Int64 | Μέγεθος xz μπλοκ αρχείου. |
| checkType | XzCheckType | Τύπος υπολογισμού αθροίσματος ελέγχου για ασυμπίεστα δεδομένα. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | *blockSize* είναι αρνητικό. |
| ArgumentNullException | *filters* είναι μηδενικό |
| ArgumentException | *filters* έχει λιγότερα από ένα ή περισσότερα από δύο φίλτρα ή το τελευταίο φίλτρο δεν είναι[`XzLZMA2FilterSettings`](../../xzlzma2filtersettings/). |

### Παραδείγματα

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
* χώρος ονομάτων [Aspose.Zip.Xz.Settings](../../xzarchivesettings/)
* συνέλευση [Aspose.Zip](../../../)


