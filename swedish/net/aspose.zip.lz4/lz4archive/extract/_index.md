---
title: "Lz4Archive.Extract"
second_title: "Aspose.ZIP för .NET API-referens"
description: "Lz4Archive-metod. Extraherar arkivet till filen enligt sökväg"
type: docs
weight: 30
url: /sv/net/aspose.zip.lz4/lz4archive/extract/
---
## Extract(string) {#extract}

Extraherar arkivet till filen via sökväg.

```csharp
public FileInfo Extract(string path)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sökväg | String | Sökvägen till destinationsfilen. Om filen redan finns, kommer den att skrivas över. |

### Returvärde

Information om en extraherad fil.

### Undantag

| undantag | villkor |
| --- | --- |
| EndOfStreamException | Källströmmen är för kort. |
| InvalidDataException | Felaktiga byte hittades vid avkodning. |
| NotSupportedException | Denna LZ4-version stöds inte. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |
| InvalidOperationException | Arkivet är förberett för sammansättning. |

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extraherar arkivet till den angivna strömmen.

```csharp
public void Extract(Stream destination)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| mål | Ström | Destinationsström. Måste vara skrivbar. |

### Undantag

| undantag | villkor |
| --- | --- |
| ArgumentException | *destination* stöder inte skrivning. |
| EndOfStreamException | Källströmmen är för kort. |
| InvalidDataException | Felaktiga byte hittades vid avkodning. |
| NotSupportedException | Denna LZ4-version stöds inte. |
| InvalidOperationException | Arkivet är förberett för sammansättning. |
| OperationCanceledException | I .NET Framework 4.0 och senare: Kastas när extraktionen avbryts via den angivna avbokningstoken. |
| ObjectDisposedException | Arkivet har frigjorts och kan inte användas. |

## Exempel

```csharp
using (var archive = new Lz4Archive("archive.lz4"))
{
     archive.Extract(httpResponseStream);
}
```

### Se även

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


