---
title: GzipArchive.SetSource
second_title: Aspose.ZIP voor .NET API-referentie
description: GzipArchive methode. Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.
type: docs
weight: 70
url: /nl/net/aspose.zip.gzip/gziparchive/setsource/
---
## SetSource(Stream) {#setsource_2}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| source | Stream | De invoerstroom voor het archief. |

### Voorbeelden

```csharp
using (var archive = new GzipArchive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.gz");
}
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileInfo | FileInfo | De verwijzing naar een te comprimeren bestand. |

### Voorbeelden

Open een archief vanuit een stream en pak het uit naar een`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.gz");
}
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Pad naar te comprimeren bestand. |

### Uitzonderingen

| uitzondering | voorwaarde |
| --- | --- |
| ArgumentNullException | *path* is niets. |
| SecurityException | De beller heeft niet de vereiste toegangsrechten. |
| ArgumentException | De*path* is leeg, bevat alleen spaties of bevat ongeldige tekens. |
| UnauthorizedAccessException | Toegang tot dossier*path* wordt ontkend. |
| PathTooLongException | De opgegeven*path*, bestandsnaam of beide overschrijden de door het systeem gedefinieerde maximale lengte. Op Windows-gebaseerde platforms moeten paden bijvoorbeeld uit minder dan 248 tekens bestaan en moeten bestandsnamen uit minder dan 260 tekens bestaan. |
| NotSupportedException | Dossier bij*path* bevat een dubbele punt (:) in het midden van de tekenreeks. |

### Voorbeelden

Open een archief vanuit bestand op pad en pak het uit naar een`MemoryStream`

```csharp
using (var archive = new GzipArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.gz");
}
```

### Zie ook

* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)

---

## SetSource(TarArchive) {#setsource}

Stelt de inhoud in die binnen het archief moet worden gecomprimeerd.

```csharp
public void SetSource(TarArchive tarArchive)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| tarArchive | TarArchive | Tar-archief dat moet worden gecomprimeerd. |

### Opmerkingen

Gebruik deze methode om een gezamenlijk tar.gz-archief samen te stellen.

### Voorbeelden

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var gzippedArchive = new GzipArchive())
    {
           gzippedArchive.SetSource(tarArchive);
           gzippedArchive.Save("archive.tar.gz");
    }
}
```

### Zie ook

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* class [GzipArchive](../)
* naamruimte [Aspose.Zip.Gzip](../../gziparchive/)
* montage [Aspose.Zip](../../../)


