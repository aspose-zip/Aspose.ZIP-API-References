---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP för .NET API-referens"
description: "AppleArchive‑metod. Sparar arkivet till den angivna strömmen."
type: docs
weight: 90
url: /sv/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Sparar arkivet till den angivna strömmen.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Ström | Målsström. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har avlägsnats. |
| ArgumentNullException | *output* är `null`. |
| ArgumentException | *output* är inte skrivbar. |
| ArgumentOutOfRangeException | Konfigurerad LZ4‑ eller Zlib‑blockstorlek är inte positiv. |
| NotSupportedException | Komprimeringsinställningar saknas eller stöds inte, direktkomposition använder en icke‑sökbar ström, eller så överskrider post/arkivstorlek nuvarande gränser för Apple‑arkivet. |

## Anmärkningar

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Se även

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Sparar arkivet till en angiven destinationsfil.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| destinationFileName | String | Sökvägen till arkivet som ska skapas. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har avlägsnats. |
| ArgumentException | *destinationFileName* är ogiltig. |
| ArgumentNullException | *destinationFileName* är `null`. |
| ArgumentOutOfRangeException | Konfigurerad LZ4‑ eller Zlib‑blockstorlek är inte positiv. |
| NotSupportedException | Komprimeringsinställningar saknas eller stöds inte, direktkomposition använder en icke‑sökbar ström, eller så överskrider post/arkivstorlek nuvarande gränser för Apple‑arkivet. |

### Se även

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


