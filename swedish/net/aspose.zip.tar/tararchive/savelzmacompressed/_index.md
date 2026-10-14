---
title: "TarArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "TarArchive-metod. Sparar arkivet till strömmen med LZMA-komprimering"
type: docs
weight: 190
url: /sv/net/aspose.zip.tar/tararchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, TarFormat?) {#savelzmacompressed}

Sparar arkivet till strömmen med LZMA-komprimering.

```csharp
public void SaveLZMACompressed(Stream output, TarFormat? format = default)
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

Viktigt: tar-arkivet skapas och komprimeras sedan inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

## Exempel

```csharp
using (FileStream result = File.OpenWrite("result.tar.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
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

## SaveLZMACompressed(string, TarFormat?) {#savelzmacompressed_1}

Sparar arkivet till filen via sökväg med lzma-komprimering.

```csharp
public void SaveLZMACompressed(string path, TarFormat? format = default)
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

## Anmärkningar

Viktigt: tar-arkivet skapas och komprimeras sedan inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

## Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.tar.lzma");
    }
}
```

### Se även

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


