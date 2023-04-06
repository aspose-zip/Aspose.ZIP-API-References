---
title: TarArchive.SaveGzipped
second_title: Aspose.ZIP για Αναφορά API .NET
description: TarArchive μέθοδος. Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip.
type: docs
weight: 130
url: /el/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

Αποθηκεύει το αρχείο στη ροή με συμπίεση gzip.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| output | Stream | Ροή προορισμού. |
| format | Nullable`1 | Καθορίζει τη μορφή κεφαλίδας tar. Η μηδενική τιμή θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentNullException | *output* είναι μηδενικό. |
| ArgumentException | *output* δεν είναι εγγράψιμο. |

### Παρατηρήσεις

*output*πρέπει να είναι εγγράψιμο.

### Παραδείγματα

```csharp
using (FileStream result = File.OpenWrite("result.tar.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Δείτε επίσης

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

Αποθηκεύει το αρχείο στο αρχείο κατά διαδρομή με συμπίεση gzip.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| path | String | Η διαδρομή του αρχείου που θα δημιουργηθεί. Εάν το καθορισμένο όνομα αρχείου παραπέμπει σε ένα υπάρχον αρχείο, θα αντικατασταθεί. |
| format | Nullable`1 | Καθορίζει τη μορφή κεφαλίδας tar. Η μηδενική τιμή θα αντιμετωπίζεται ως USTar όταν είναι δυνατόν. |

### Παραδείγματα

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### Δείτε επίσης

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* χώρος ονομάτων [Aspose.Zip.Tar](../../tararchive/)
* συνέλευση [Aspose.Zip](../../../)


