---
title: "Bzip2SaveOptions.Bzip2SaveOptions"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Κατασκευαστής Bzip2SaveOptions. Αρχικοποιεί μια νέα παρουσία της κλάσης Bzip2SaveOptions"
type: docs
weight: 10
url: /el/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Bzip2SaveOptions`](../).

```csharp
public Bzip2SaveOptions(int blockSize)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| blockSize | Int32 | Μέγεθος μπλοκ σε εκατοντάδες kilobytes. |

### Εξαιρέσεις

| εξαίρεση | συνθήκη |
| --- | --- |
| ArgumentOutOfRangeException | Το μέγεθος μπλοκ δεν βρίσκεται σε έγκυρο εύρος. |

## Παραδείγματα

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
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

Αρχικοποιεί μια νέα παρουσία της κλάσης [`Bzip2SaveOptions`](../) με προεπιλεγμένο μέγεθος μπλοκ, ίσο με 9 εκατοντάδες kilobytes.

```csharp
public Bzip2SaveOptions()
```

## Παραδείγματα

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
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


