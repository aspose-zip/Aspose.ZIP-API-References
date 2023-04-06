---
title: GzipArchive.Extract
second_title: Aspose.ZIP για Αναφορά API .NET
description: GzipArchive μέθοδος. Εξάγει το αρχείο στη ροή που παρέχεται.
type: docs
weight: 40
url: /el/net/aspose.zip.gzip/gziparchive/extract/
---
## GzipArchive.Extract method

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
using (var archive = new GzipArchive("archive.gz"))
{
     archive.Extract(httpResponseStream);
}
```

### Δείτε επίσης

* class [GzipArchive](../)
* χώρος ονομάτων [Aspose.Zip.Gzip](../../gziparchive/)
* συνέλευση [Aspose.Zip](../../../)


