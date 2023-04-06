---
title: SevenZipLZMA2CompressionSettings.SevenZipLZMA2CompressionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipLZMA2CompressionSettings constructeur. Instanziiert Einstellungen für die LZMA2Komprimierungsmethode innerhalb des 7zArchivs.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/sevenziplzma2compressionsettings/sevenziplzma2compressionsettings/
---
## SevenZipLZMA2CompressionSettings(int) {#constructor}

Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb des 7z-Archivs.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize = 16777216)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dictionarySize | Int32 | Größe des Verlaufspuffers, muss zwischen 4096 und 1073741824 liegen. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* ist zu groß oder zu klein. |

### Bemerkungen

Je größer das Wörterbuch ist, desto besser ist normalerweise das Komprimierungsverhältnis, aber Wörterbücher, die größer sind als die unkomprimierten Daten, sind eine Verschwendung von RAM.

### Siehe auch

* class [SevenZipLZMA2CompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* Montage [Aspose.Zip](../../../)

---

## SevenZipLZMA2CompressionSettings(int, int) {#constructor_1}

Instanziiert Einstellungen für die LZMA2-Komprimierungsmethode innerhalb des 7z-Archivs.

```csharp
public SevenZipLZMA2CompressionSettings(int dictionarySize, int fastBytes = 32)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| dictionarySize | Int32 | Größe des Verlaufspuffers, muss zwischen 4096 und 1073741824 liegen. |
| fastBytes | Int32 | Steuert die Anzahl der schnellen Bytes, die von den LZMA2-Kompressoren verwendet werden. Eine größere Anzahl schneller Bytes kann ein besseres Komprimierungsverhältnis auf Kosten der Komprimierungsgeschwindigkeit bereitstellen. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | *dictionarySize* ist zu groß oder zu klein, bzw*fastBytes* ist zu groß oder zu klein. |

### Bemerkungen

Je größer das Wörterbuch ist, desto besser ist normalerweise das Komprimierungsverhältnis, aber Wörterbücher, die größer sind als die unkomprimierten Daten, sind eine Verschwendung von RAM.

### Siehe auch

* class [SevenZipLZMA2CompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../sevenziplzma2compressionsettings/)
* Montage [Aspose.Zip](../../../)


