---
title: "AlzArchive.AlzArchive"
second_title: "Aspose.ZIP für .NET API-Referenz"
description: "AlzArchive-Konstruktor. Initialisiert eine neue Instanz der Klasse AlzArchive aus einem Stream"
type: docs
weight: 10
url: /de/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Initialisiert eine neue Instanz der [`AlzArchive`](../)-Klasse aus einem Stream.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| stream | Stream | Der ALZ-Archiv-Stream. Der Stream muss das Lesen und Suchen unterstützen. |
| loadOptions | AlzArchiveLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Stream ist null. |

### Siehe auch

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Initialisiert eine neue Instanz der [`AlzArchive`](../)-Klasse aus einem Dateipfad.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Dateipfad | String | Pfad zur ALZ-Archivdatei. |
| loadOptions | AlzArchiveLoadOptions | Optionen zum Laden eines vorhandenen Archivs. |

### Ausnahmen

| Ausnahme | Bedingung |
| --- | --- |
| ArgumentNullException | Dateipfad ist null. |
| FileNotFoundException | Die Datei existiert nicht. |

### Siehe auch

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


