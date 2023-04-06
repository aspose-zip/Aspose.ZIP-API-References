---
title: RarArchive.RarArchive
second_title: Aspose.ZIP voor .NET API-referentie
description: RarArchive constructeur. Initialiseert een nieuw exemplaar van hetRarArchive klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.
type: docs
weight: 10
url: /nl/net/aspose.zip.rar/rararchive/rararchive/
---
## RarArchive(string, RarArchiveLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`RarArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public RarArchive(string path, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het volledig gekwalificeerde of relatieve pad naar het archiefbestand. |
| loadOptions | RarArchiveLoadOptions | Opties om bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Opmerkingen

Deze constructor decomprimeert geen enkel item. Zien[`Open`](../../rararchiveentry/open/) methode voor decomprimeren.

### Voorbeelden

Het volgende voorbeeld extraheert een archief en decomprimeert vervolgens het eerste item naar een`MemoryStream`.

```csharp
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive("data.rar"))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Zie ook

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* naamruimte [Aspose.Zip.Rar](../../rararchive/)
* montage [Aspose.Zip](../../../)

---

## RarArchive(Stream, RarArchiveLoadOptions) {#constructor}

Initialiseert een nieuw exemplaar van het[`RarArchive`](../) klasse en lijst met items voor samenstellen kunnen uit het archief worden geëxtraheerd.

```csharp
public RarArchive(Stream sourceStream, RarArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |
| loadOptions | RarArchiveLoadOptions | Opties om bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentException | *sourceStream* is niet zoek. |
| InvalidDataException | Verkeerde handtekening voor archief. - of - Het bestand is geen RAR-archief. |
| InvalidOperationException |  |

### Opmerkingen

Deze constructor decomprimeert geen enkel item. Zien[`Open`](../../rararchiveentry/open/) methode voor decomprimeren.

### Voorbeelden

In het volgende voorbeeld wordt de eerste invoer van a ontcijferd en gedecomprimeerd`MemoryStream`.

```csharp
var fs = File.OpenRead("encrypted.rar");
var extracted = new MemoryStream();
using (RarArchive archive = new RarArchive(fs, new RarArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
{
    using (var decompressed = archive.Entries[0].Open())
    {
        byte[] b = new byte[8192];
        int bytesRead;
        while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
            extracted.Write(b, 0, bytesRead);
    }
}
```

### Zie ook

* class [RarArchiveLoadOptions](../../rararchiveloadoptions/)
* class [RarArchive](../)
* naamruimte [Aspose.Zip.Rar](../../rararchive/)
* montage [Aspose.Zip](../../../)


