---
title: TarArchive.FromLZip
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Extraherar medföljande lziparkiv och komponerarTarArchive från extraherade data.
type: docs
weight: 30
url: /sv/net/aspose.zip.tar/tararchive/fromlzip/
---
## FromLZip(Stream) {#fromlzip}

Extraherar medföljande lzip-arkiv och komponerar[`TarArchive`](../) från extraherade data.

Viktigt: lzip-arkivet är helt extraherat inom denna metod, dess innehåll bevaras internt. Akta dig för minnesförbrukning.

```csharp
public static TarArchive FromLZip(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | Stream | Källan till arkivet. |

### Returvärde

Ett exempel på[`TarArchive`](../)

### Anmärkningar

Lzip-extraktionsström är inte sökbar av komprimeringsalgoritmens natur. Tar-arkivet ger möjlighet att extrahera godtyckliga register, så det måste driva sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## FromLZip(string) {#fromlzip_1}

Extraherar medföljande lzip-arkiv och komponerar[`TarArchive`](../) från extraherade data.

Viktigt: lzip-arkivet är helt extraherat inom denna metod, dess innehåll bevaras internt. Akta dig för minnesförbrukning.

```csharp
public static TarArchive FromLZip(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivfilen. |

### Returvärde

Ett exempel på[`TarArchive`](../)

### Anmärkningar

Lzip-extraktionsström är inte sökbar av komprimeringsalgoritmens natur. Tar-arkivet ger möjlighet att extrahera godtyckliga register, så det måste driva sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


