---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "CpioArchive-metod. Sparar arkivet till strömmen med LZMA-komprimering"
type: docs
weight: 110
url: /sv/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

Sparar arkivet till strömmen med LZMA-komprimering.

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Ström | Målsström. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| NotSupportedException | Strömmen stöder inte skrivning, eller så är strömmen redan stängd. |

## Anmärkningar

*output* must be writable.

Viktigt: cpio-arkivet byggs upp och komprimeras sedan inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

## Exempel

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

Sparar arkivet till filen via sökväg med lzma-komprimering.

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentNullException | *path* är `null`. |
| Undantag | Kastas när ett körningsfel inträffar. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig (till exempel om den ligger på en ej mappad enhet). |
| IOException | Ett I/O‑fel inträffar. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider systemdefinierad maximal längd. |
| UnauthorizedAccessException | Anroparen har inte den nödvändiga behörigheten. -eller- *path* angav en skrivskyddad fil eller katalog. |

## Anmärkningar

Viktigt: cpio-arkivet byggs upp och komprimeras sedan inom denna metod, dess innehåll behålls internt. Var medveten om minnesanvändning.

## Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


