---
title: SharArchive.SharArchive
second_title: Aspose.ZIP för .NET API-referens
description: SharArchive byggare. Initierar en ny instans avSharArchive class.
type: docs
weight: 10
url: /sv/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Initierar en ny instans av[`SharArchive`](../) class.

```csharp
public SharArchive()
```

### Exempel

Följande exempel visar hur man komprimerar en fil.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Se även

* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Se även

* class [SharArchive](../)
* namnutrymme [Aspose.Zip.Shar](../../shararchive/)
* hopsättning [Aspose.Zip](../../../)


