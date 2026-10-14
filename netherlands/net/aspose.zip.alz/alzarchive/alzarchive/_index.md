---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AlzArchive constructor. Initialiseert een nieuw exemplaar van de AlzArchive klasse vanuit een stream"
type: docs
weight: 10
url: /nl/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Initialiseert een nieuw exemplaar van de [`AlzArchive`](../) klasse vanuit een stream.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| stream | Stream | De ALZ-archiefstream. De stream moet lezen en zoeken ondersteunen. |
| loadOptions | AlzArchiveLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | stream is null. |

### Zie ook

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Initialiseert een nieuw exemplaar van de [`AlzArchive`](../) klasse vanuit een bestandspad.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| filePath | String | Pad naar het ALZ-archiefbestand. |
| loadOptions | AlzArchiveLoadOptions | Opties om een bestaand archief mee te laden. |

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ArgumentNullException | filePath is null. |
| FileNotFoundException | Het bestand bestaat niet. |

### Zie ook

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


