---
title: "IsoArchive.CreateDirectory"
second_title: "Aspose.ZIP för .NET API-referens"
description: "IsoArchive‑metod. Lägger till en katalog i ISO‑avbilden"
type: docs
weight: 30
url: /sv/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Lägger till en katalog i ISO-avbilden.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | String | Sökväg till katalogen i ISO:n. |

### Returvärde

ISO‑posten har sammansatts.

### Undantag

| undantag | villkor |
| --- | --- |
| InvalidOperationException | Arkivet är öppnat för extraktion. |
| ArgumentNullException | `name` är null eller tom. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

### Se även

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


