---
title: SharArchive.SharArchive
second_title: Aspose.ZIP για Αναφορά API .NET
description: SharArchive κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουSharArchive τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`SharArchive`](../) τάξη.

```csharp
public SharArchive()
```

### Παραδείγματα

Το ακόλουθο παράδειγμα δείχνει τον τρόπο συμπίεσης ενός αρχείου.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Δείτε επίσης

* class [SharArchive](../)
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Δείτε επίσης

* class [SharArchive](../)
* χώρος ονομάτων [Aspose.Zip.Shar](../../shararchive/)
* συνέλευση [Aspose.Zip](../../../)


