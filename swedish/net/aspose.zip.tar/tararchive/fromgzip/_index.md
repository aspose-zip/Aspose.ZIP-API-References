---
title: TarArchive.FromGZip
second_title: Aspose.ZIP för .NET API-referens
description: TarArchive metod. Extraherar medföljande gziparkiv och komponerarTarArchive från extraherade data.
type: docs
weight: 20
url: /sv/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Extraherar medföljande gzip-arkiv och komponerar[`TarArchive`](../) från extraherade data.

Viktigt: gzip-arkivet är helt extraherat inom denna metod, dess innehåll bevaras internt. Akta dig för minnesförbrukning.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| source | Stream | Källan till arkivet. |

### Returvärde

Ett exempel på[`TarArchive`](../)

### Anmärkningar

GZip-extraktionsströmmen är inte sökbar på grund av kompressionsalgoritmens natur. Tar-arkivet ger möjlighet att extrahera godtyckliga uppgifter, så det måste drivas sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Extraherar medföljande gzip-arkiv och komponerar[`TarArchive`](../) från extraherade data.

Viktigt: gzip-arkivet är helt extraherat inom denna metod, dess innehåll bevaras internt. Akta dig för minnesförbrukning.

```csharp
public static TarArchive FromGZip(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| path | String | Sökvägen till arkivfilen. |

### Returvärde

Ett exempel på[`TarArchive`](../)

### Anmärkningar

GZip-extraktionsströmmen är inte sökbar på grund av kompressionsalgoritmens natur. Tar-arkivet ger möjlighet att extrahera godtyckliga uppgifter, så det måste drivas sökbar ström under huven.

### Se även

* class [TarArchive](../)
* namnutrymme [Aspose.Zip.Tar](../../tararchive/)
* hopsättning [Aspose.Zip](../../../)


