---
title: SharArchive.SharArchive
second_title: Aspose.ZIP für .NET-API-Referenz
description: SharArchive constructeur. Initialisiert eine neue Instanz vonSharArchive Klasse.
type: docs
weight: 10
url: /de/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Initialisiert eine neue Instanz von[`SharArchive`](../) Klasse.

```csharp
public SharArchive()
```

### Beispiele

Das folgende Beispiel zeigt, wie eine Datei komprimiert wird.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Siehe auch

* class [SharArchive](../)
* namensraum [Aspose.Zip.Shar](../../shararchive/)
* Montage [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Siehe auch

* class [SharArchive](../)
* namensraum [Aspose.Zip.Shar](../../shararchive/)
* Montage [Aspose.Zip](../../../)


