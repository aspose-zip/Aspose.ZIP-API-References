---
title: "TarArchive.SaveLZ4Compressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "TarArchive-metod. Sparar arkivet till strömmen med LZ4-komprimering"
type: docs
weight: 170
url: /sv/net/aspose.zip.tar/tararchive/savelz4compressed/
---
## SaveLZ4Compressed(Stream, TarFormat?) {#savelz4compressed}

Sparar arkivet till strömmen med LZ4-komprimering.

```csharp
public void SaveLZ4Compressed(Stream output, TarFormat? format = default)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Ström | Målsström. |
| format | Nullable`1 | Definierar tar-huvudformatet. Nullvärde kommer att behandlas som USTar när det är möjligt. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *output* är null. |
| ArgumentException | *output* är inte skrivbar. |
| ObjectDisposedException | Arkivet har avlägsnats och kan inte användas |
| IOException | Ett I/O‑fel inträffar. |

## Anmärkningar

*output* must be writable.

## Exempel

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz4"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZ4Compressed(result);
        }
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZ4Compressed(string, TarFormat?) {#savelz4compressed_1}

Sparar arkivet till filen via sökväg med LZ4-komprimering.

```csharp
public void SaveLZ4Compressed(string path, TarFormat? format = default)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| format | Nullable`1 | Definierar tar-huvudformatet. Nullvärde kommer att behandlas som USTar när det är möjligt. |

### Undantag

| undantag | villkor |
| --- | --- |
| UnauthorizedAccessException | Anroparen har inte den nödvändiga behörigheten. -eller- *path* angav en skrivskyddad fil eller katalog. |
| ArgumentException | *path* är en sträng med noll längd, innehåller bara blanksteg, eller innehåller en eller flera ogiltiga tecken enligt InvalidPathChars. |
| ArgumentNullException | *path* är null. |
| PathTooLongException | Den angivna *path*, filnamnet eller båda överskrider systemdefinierad maximal längd. Till exempel, på Windows-baserade plattformar måste sökvägar vara kortare än 248 tecken och filnamn kortare än 260 tecken. |
| DirectoryNotFoundException | Den angivna *path* är ogiltig, (till exempel eftersom den ligger på en omappad enhet). |
| NotSupportedException | *path* har ett ogiltigt format. |
| ObjectDisposedException | Arkivet har avlägsnats och kan inte användas |
| IOException | Ett I/O‑fel inträffar. |

## Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZ4Compressed("result.tar.lz4");
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


