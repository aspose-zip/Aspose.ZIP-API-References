---
title: "CpioArchive.SaveZCompressed"
second_title: "Aspose.ZIP för .NET API-referens"
description: "CpioArchive-metod. Sparar arkivet till strömmen med Z-komprimering"
type: docs
weight: 130
url: /sv/net/aspose.zip.cpio/cpioarchive/savezcompressed/
---
## SaveZCompressed(Stream, CpioFormat) {#savezcompressed}

Sparar arkivet till strömmen med Z-komprimering.

```csharp
public void SaveZCompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
using (FileStream result = File.OpenWrite("result.cpio.Z"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveZCompressed(result);
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

## SaveZCompressed(string, CpioFormat) {#savezcompressed_1}

Sparar arkivet till sökvägen med Z-komprimering.

```csharp
public void SaveZCompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
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
| DirectoryNotFoundException | Den angivna sökvägen är ogiltig (till exempel om den ligger på en ej mappad enhet). |
| IOException | Ett I/O‑fel inträffar. |
| PathTooLongException | Den angivna sökvägen, filnamnet eller båda överskrider systemdefinierad maximal längd. |

## Exempel

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveZCompressed("result.cpio.Z");
    }
}
```

### Se även

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


