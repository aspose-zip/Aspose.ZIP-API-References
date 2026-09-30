---
title: "GzipArchive.UncompressedSize"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "GzipArchive ιδιότητα. Λαμβάνει το μέγεθος ενός αρχικού αρχείου"
type: docs
weight: 30
url: /el/net/aspose.zip.gzip/gziparchive/uncompressedsize/
---
## GzipArchive.UncompressedSize property

Λαμβάνει το μέγεθος ενός αρχικού αρχείου.

```csharp
public ulong UncompressedSize { get; }
```

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ObjectDisposedException | Το αρχείο έχει διαγραφεί και δεν μπορεί να χρησιμοποιηθεί. |

## Παρατηρήσεις

Κατά τη διάρκεια της αποσυμπίεσης, αυτή η ιδιότητα ενδέχεται να περιέχει λανθασμένο μέγεθος. Εάν το μέγεθος του αποσυμπιεσμένου αρχείου υπερβαίνει τα 4 GB, αυτή η ιδιότητα θα δώσει λανθασμένη τιμή λόγω του 32‑bit ορίου στην κεφαλίδα.

### Δείτε επίσης

* class [GzipArchive](../)
* namespace [Aspose.Zip.Gzip](../../gziparchive/)
* assembly [Aspose.Zip](../../../)


