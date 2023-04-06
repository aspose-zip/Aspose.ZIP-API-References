---
title: CpioArchive.SaveXzCompressed
second_title: Aspose.ZIP για Αναφορά API .NET
description: CpioArchive μέθοδος. Αποθηκεύει το αρχείο στη ροή με συμπίεση xz.
type: docs
weight: 100
url: /el/net/aspose.zip.cpio/cpioarchive/savexzcompressed/
---
## SaveXzCompressed(Stream, CpioFormat, XzArchiveSettings) {#savexzcompressed}

Αποθηκεύει το αρχείο στη ροή με συμπίεση xz.

```csharp
public void SaveXzCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| cpioFormat | CpioFormat | Καθορίζει τη μορφή κεφαλίδας cpio. |
| settings | XzArchiveSettings | Σύνολο ρύθμισης συγκεκριμένου αρχείου xz: μέγεθος λεξικού, μέγεθος μπλοκ, τύπος ελέγχου. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *output* είναι μηδενικό. |
| ArgumentException | *output* δεν είναι εγγράψιμο. |

### Παρατηρήσεις

*output*Η ροή πρέπει να είναι εγγράψιμη.

### Παραδείγματα

```csharp
using (FileStream result = File.OpenWrite("result.cpio.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, CpioFormat, XzArchiveSettings) {#savexzcompressed_1}

Αποθηκεύει το αρχείο στη διαδρομή ανά διαδρομή με συμπίεση xz.

```csharp
public void SaveXzCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii, 
    XzArchiveSettings settings = null)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |
| cpioFormat | CpioFormat | Καθορίζει τη μορφή κεφαλίδας cpio. |
| settings | XzArchiveSettings | Σύνολο ρύθμισης συγκεκριμένου αρχείου xz: μέγεθος λεξικού, μέγεθος μπλοκ, τύπος ελέγχου. |

### Παραδείγματα

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.cpio.xz");
    }
}
```

### Δείτε επίσης

* enum [CpioFormat](../../cpioformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [CpioArchive](../)
* χώρος ονομάτων [Aspose.Zip.Cpio](../../cpioarchive/)
* συνέλευση [Aspose.Zip](../../../)


