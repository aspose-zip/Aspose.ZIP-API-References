---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP για Αναφορά API .NET
description: Bzip2SaveOptions κατασκευαστής. Αρχικοποιεί μια νέα παρουσία τουBzip2SaveOptions τάξη.
type: docs
weight: 10
url: /el/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία του[`Bzip2SaveOptions`](../) τάξη.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | Int32 | Μέγεθος μπλοκ σε εκατοντάδες kilobyte. |

### Εξαιρέσεις

| εξαίρεση | κατάσταση |
| --- | --- |
| ArgumentOutOfRangeException | Το μέγεθος του μπλοκ δεν είναι σε έγκυρο εύρος. |

### Παραδείγματα

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### Δείτε επίσης

* class [Bzip2SaveOptions](../)
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* συνέλευση [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Αρχικοποιεί μια νέα παρουσία του[`Bzip2SaveOptions`](../) κλάση με προεπιλεγμένο μέγεθος μπλοκ, ισούται με 9 εκατοντάδες kilobyte.

```csharp
public Bzip2SaveOptions()
```

### Παραδείγματα

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### Δείτε επίσης

* class [Bzip2SaveOptions](../)
* χώρος ονομάτων [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* συνέλευση [Aspose.Zip](../../../)


