---
title: SharArchive.SharArchive
second_title: Riferimento API Aspose.ZIP per .NET
description: SharArchive costruttore. Inizializza una nuova istanza diSharArchive classe.
type: docs
weight: 10
url: /it/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Inizializza una nuova istanza di[`SharArchive`](../) classe.

```csharp
public SharArchive()
```

### Esempi

L'esempio seguente mostra come comprimere un file.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Guarda anche

* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Guarda anche

* class [SharArchive](../)
* spazio dei nomi [Aspose.Zip.Shar](../../shararchive/)
* assemblea [Aspose.Zip](../../../)


