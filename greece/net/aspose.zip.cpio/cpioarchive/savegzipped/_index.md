---
title: CpioArchive.SaveGzipped
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioArchive μέθοδος. Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip.
type: docs
weight: 90
url: /el/net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip.

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| cpioFormat | CpioFormat | Καθορίζει τη μορφή κεφαλίδας cpio. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *output* είναι μηδενικό. |
| ArgumentException | *output* δεν είναι εγγράψιμο. |

### Παρατηρήσεις

*output*πρέπει να είναι εγγράψιμο.

### Παραδείγματα

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

Αποθηκεύει το αρχείο στο αρχείο κατά διαδρομή με συμπίεση gzip.

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |
| cpioFormat | CpioFormat | Καθορίζει τη μορφή κεφαλίδας cpio. |

### Παραδείγματα

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)


