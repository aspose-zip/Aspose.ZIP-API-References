---
title: Bzip2Archive.Bzip2Archive
second_title: Aspose.ZIP voor .NET API-referentie
description: Bzip2Archive constructeur. Initialiseert een nieuw exemplaar van hetBzip2Archive klasse voorbereid voor compressie.
type: docs
weight: 10
url: /nl/net/aspose.zip.bzip2/bzip2archive/bzip2archive/
---
## Bzip2Archive() {#constructor}

Initialiseert een nieuw exemplaar van het[`Bzip2Archive`](../) klasse voorbereid voor compressie.

```csharp
public Bzip2Archive()
```

### Voorbeelden

In het volgende voorbeeld ziet u hoe u een bestand kunt comprimeren.

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)

---

## Bzip2Archive(Stream) {#constructor_1}

Initialiseert een nieuw exemplaar van het[`Bzip2Archive`](../) klasse voorbereid voor decomprimeren.

```csharp
public Bzip2Archive(Stream sourceStream)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| sourceStream | Stream | De bron van het archief. |

### Opmerkingen

Deze constructor decomprimeert niet. Zien[`Open`](../open/) methode voor decomprimeren.

### Voorbeelden

Open een archief vanuit een stream en pak het uit naar een`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive(File.OpenRead("archive.bz2")))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)

---

## Bzip2Archive(string) {#constructor_2}

Initialiseert een nieuw exemplaar van het[`Bzip2Archive`](../) klasse voorbereid voor decomprimeren.

```csharp
public Bzip2Archive(string path)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| path | String | Het pad naar het archiefbestand. |

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

Deze constructor decomprimeert niet. Zien[`Open`](../open/) methode voor decomprimeren.

### Voorbeelden

Open een archief vanuit bestand op pad en pak het uit naar een`MemoryStream`

```csharp
var ms = new MemoryStream();
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
  archive.Open().CopyTo(ms);
```

### Zie ook

* class [Bzip2Archive](../)
* naamruimte [Aspose.Zip.Bzip2](../../bzip2archive/)
* montage [Aspose.Zip](../../../)


