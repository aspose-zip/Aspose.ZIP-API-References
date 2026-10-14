---
title: "CpioArchive.SaveZstandard"
second_title: "Aspose.ZIP för .NET API-referens"
description: "CpioArchive-metod. Sparar arkivet till strömmen med Zstandard-komprimering"
type: docs
weight: 140
url: /sv/net/aspose.zip.cpio/cpioarchive/savezstandard/
---
## SaveZstandard(Stream, CpioFormat) {#savezstandard}

Sparar arkivet till strömmen med Zstandard-komprimering.

```csharp
public void SaveZstandard(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| output | Ström | Målsström. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentNullException | *output* är null. |
| ArgumentException | *output* är inte skrivbar. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Anmärkningar

*output* must be writable.

## Exempel

```csharp
using (FileStream result = File.OpenWrite("result.cpio.zst"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZstandard(result);
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

## SaveZstandard(string, CpioFormat) {#savezstandard_1}

Sparar arkivet till filen via sökväg med Zstandard-komprimering.

```csharp
public void SaveZstandard(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen för arkivet som ska skapas. Om det angivna filnamnet pekar på en befintlig fil kommer den att skrivas över. |
| cpioFormat | CpioFormat | Definierar cpio-huvudformat. |

### Undantag

| undantag | villkor |
| --- | --- |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| ArgumentException | *path* är en sträng med noll längd, innehåller bara blanksteg, eller innehåller en eller flera ogiltiga tecken enligt InvalidPathChars. |
| ArgumentNullException | *path* är `null`. |
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig (till exempel om den ligger på en ej mappad enhet). |
| IOException | Ett I/O‑fel inträffar. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider systemdefinierad maximal längd. |
| UnauthorizedAccessException | Anroparen har inte den nödvändiga behörigheten. -eller- *path* angav en skrivskyddad fil eller katalog. |

## Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZstandard("result.cpio.zst");
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


