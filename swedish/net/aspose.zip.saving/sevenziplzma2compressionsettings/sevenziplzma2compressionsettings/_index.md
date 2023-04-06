---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP för .NET API-referens
description: SevenZipLZMA2CompressionSettings byggare. Instantierar inställningar för LZMA2komprimeringsmetod inom 7zarkiv.
type: docs
weight: 10
url: /sv/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Instantierar inställningar för LZMA2-komprimeringsmetod inom 7z-arkiv.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dictionarySize | Int32 | Storlek på historikbuffert, måste vara mellan 4096 och 1073741824. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* är för stor eller för liten. |

### Anmärkningar

Ju större ordboken är, desto bättre är komprimeringsförhållandet vanligtvis, men ordböcker som är större än okomprimerade data är slöseri med RAM.

### Se även

* class [SevenZipLZMA2CompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* hopsättning [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Instantierar inställningar för LZMA2-komprimeringsmetod inom 7z-arkiv.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| dictionarySize | Int32 | Storlek på historikbuffert, måste vara mellan 4096 och 1073741824. |
| fastBytes | Int32 | Styr antalet snabba bytes som används av LZMA2-kompressorerna. Ett större antal snabba bytes kan ge ett bättre kompressionsförhållande på bekostnad av kompressionshastigheten. |

### Undantag

| undantag | skick |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* är för stor eller för liten, eller*fastBytes* är för stor eller för liten. |

### Anmärkningar

Ju större ordboken är, desto bättre är komprimeringsförhållandet vanligtvis, men ordböcker som är större än okomprimerade data är slöseri med RAM.

### Se även

* class [SevenZipLZMA2CompressionSettings](../)
* namnutrymme [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* hopsättning [Aspose.Zip](../../../)


