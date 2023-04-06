---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP für .NET-API-Referenz
description: SevenZipPPMdCompressionSettings constructeur. Instanziiert Einstellungen für die PPMdKomprimierungsmethode innerhalb des 7zArchivs.
type: docs
weight: 10
url: /de/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Instanziiert Einstellungen für die PPMd-Komprimierungsmethode innerhalb des 7z-Archivs.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| maxOrder | Byte | Maximale Bestellung. |
| suballocatorSize | Int32 | Die Speichergröße in MB kann vom Suballocator verbraucht werden. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* liegt nicht zwischen 2 und 32, bzw*suballocatorSize* liegt nicht zwischen 1 und 1024. |

### Bemerkungen

Größere Modellbestellungen führen fast sicher zu einer besseren Komprimierung und sicherlich zu mehr Speicher- und CPU-Auslastung.

Der PPMd-Algorithmus benötigt möglicherweise viel Speicher, insbesondere wenn er mit großen Dateien und/oder mit einer großen Modellreihenfolge verwendet wird. Wenn ppmd mehr Speicher benötigt, als Sie ihm geben, wird die Komprimierung schlechter.

### Beispiele

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Siehe auch

* class [SevenZipPPMdCompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* Montage [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Instanziiert Einstellungen für die PPMd-Komprimierungsmethode innerhalb des 7z-Archivs mit standardmäßiger Modellreihenfolge und Unterzuweisungsgröße.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Bemerkungen

Die Standardreihenfolge des Modells ist 6 und die Größe der Unterzuweisung ist 16 MB.

### Beispiele

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Siehe auch

* class [SevenZipPPMdCompressionSettings](../)
* namensraum [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* Montage [Aspose.Zip](../../../)


