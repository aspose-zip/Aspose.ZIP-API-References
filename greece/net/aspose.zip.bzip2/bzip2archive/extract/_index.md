---
title: Bzip2Archive.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: Bzip2Archive μέθοδος. Εξάγει το αρχείο στη ροή που παρέχεται.
type: docs
weight: 30
url: /el/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

Εξάγει το αρχείο στη ροή που παρέχεται.

```csharp
public void Extract(Stream destination)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| destination | Stream | Ροή προορισμού. Πρέπει να είναι εγγράψιμο. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentException | *destination* δεν υποστηρίζει τη γραφή. |

### Παραδείγματα

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [Bzip2Archive](../)
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2archive/)
* συνέλευση [Aspose.Zip](../../../)


