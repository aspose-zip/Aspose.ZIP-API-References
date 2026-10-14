---
title: "ArjEntryPlain.Extract"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "ArjEntryPlain method. Extraheert het item naar het bestandssysteem via het opgegeven pad"
type: docs
weight: 40
url: /nl/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Extraheert het item naar het bestandssysteem op het opgegeven pad.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| pad | String | Het pad naar het bestemmingsbestand. Als het bestand al bestaat, wordt het overschreven. |

### Retourwaarde

De bestandsinfo van een samengesteld bestand.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | *path* is null of leeg. |
| ObjectDisposedException | Wordt gegooid als het archief is vrijgegeven. |
| FileNotFoundException | Het bestand is niet gevonden. |
| InvalidDataException | Controlesom komt niet overeen voor headers of data. - of - Archief is corrupt. |
| PathTooLongException | Het opgegeven pad, bestandsnaam, of beide overschrijden de systeemgedefinieerde maximale lengte. |
| NotImplementedException | Item gecomprimeerd met methode 4. |

## Voorbeelden

Extraheer twee items van een rar-archief.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Zie ook

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extraheert een ARJ-archiefitem naar een bestand.

```csharp
public void Extract(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo voor het opslaan van gedecomprimeerde gegevens. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| InvalidOperationException | Archiefkoppen en service‑informatie zijn niet gelezen. |
| SecurityException | De aanroeper heeft niet de vereiste toestemming om de *fileInfo* te openen. |
| ArgumentException | Het bestandspad is leeg of bevat alleen witruimtes. |
| FileNotFoundException | Het bestand is niet gevonden. |
| UnauthorizedAccessException | Pad naar bestand is alleen-lezen of is een map. |
| ArgumentNullException | *fileInfo* is null. |
| DirectoryNotFoundException | Het opgegeven pad is ongeldig, bijvoorbeeld omdat het zich op een niet-toegewezen station bevindt. |
| IOException | Het bestand is al geopend. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Wordt gegooid als het archief is vrijgegeven. |
| InvalidDataException | Controlesom komt niet overeen voor headers of data. - of - Archief is corrupt. |
| NotImplementedException | Item gecomprimeerd met methode 4. |

## Voorbeelden

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Zie ook

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

Extraheert het item naar de opgegeven stream.

```csharp
public void Extract(Stream destination)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| bestemming | Stream | Bestemmingsstream. Moet schrijfbaar zijn. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentException | *destination* ondersteunt geen schrijven. |
| InvalidDataException | Controlesom komt niet overeen voor headers of data. - of - Archief is corrupt. |
| NotImplementedException | Item gecomprimeerd met methode 4. |
| OperationCanceledException | In .NET Framework 4.0 en hoger: Wordt gegooid wanneer de extractie wordt geannuleerd via het opgegeven annulerings‑token. |
| ObjectDisposedException | Wordt gegooid als het archief is vrijgegeven. |

### Zie ook

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


