---
title: "AppleArchive.Save"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AppleArchive-Methode. Speichert das Archiv in den bereitgestellten Stream."
type: docs
weight: 90
url: /de/net/aspose.zip.apple/applearchive/save/
---
## Save(Stream) {#save}

Speichert das Archiv in den bereitgestellten Stream.

```csharp
public void Save(Stream output)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Ausgabe | Stream | Ziel-Stream. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben. |
| ArgumentNullException | *output* ist `null`. |
| ArgumentException | *output* ist nicht beschreibbar. |
| ArgumentOutOfRangeException | Die konfigurierte LZ4- oder Zlib-Blockgröße ist nicht positiv. |
| NotSupportedException | Kompressionseinstellungen fehlen oder werden nicht unterstützt, direkte Komposition verwendet einen nicht suchbaren Stream, oder die Größe von Eintrag/Archiv überschreitet die aktuellen Grenzen des Apple Archive. |

## Hinweise

*output* must be writable. Some compression settings, such as LZ4, also require a seekable stream.

### Siehe auch

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Speichert das Archiv in eine bereitgestellte Zieldatei.

```csharp
public void Save(string destinationFileName)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destinationFileName | String | Der Pfad des zu erstellenden Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ObjectDisposedException | Das Archiv wurde freigegeben. |
| ArgumentException | *destinationFileName* ist ungültig. |
| ArgumentNullException | *destinationFileName* ist `null`. |
| ArgumentOutOfRangeException | Die konfigurierte LZ4- oder Zlib-Blockgröße ist nicht positiv. |
| NotSupportedException | Kompressionseinstellungen fehlen oder werden nicht unterstützt, direkte Komposition verwendet einen nicht suchbaren Stream, oder die Größe von Eintrag/Archiv überschreitet die aktuellen Grenzen des Apple Archive. |

### Siehe auch

* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


