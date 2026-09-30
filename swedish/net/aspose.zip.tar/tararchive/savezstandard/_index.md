---
title: "TarArchive.SaveZstandard"
second_title: "Aspose.ZIP för .NET API-referens"
description: "TarArchive-metod. Sparar arkivet till strömmen med Zstandard-komprimering"
type: docs
weight: 220
url: /sv/net/aspose.zip.tar/tararchive/savezstandard/
---
## SaveZstandard(Stream, TarFormat?) {#savezstandard}

Sparar arkivet till strömmen med Zstandard-komprimering.

```csharp
public void SaveZstandard(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, TarFormat?) {#savezstandard_1}

Sparar arkivet till filen via sökväg med Zstandard-komprimering.

```csharp
public void SaveZstandard(string path, TarFormat? format = default)
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

## Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.tar.zst");
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


