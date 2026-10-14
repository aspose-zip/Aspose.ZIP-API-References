---
title: "AppleArchive.CreateEntry"
second_title: "Aspose.ZIP voor .NET API-referentie"
description: "AppleArchive methode. Maakt een enkel item aan in het archief"
type: docs
weight: 60
url: /nl/net/aspose.zip.apple/applearchive/createentry/
---
## CreateEntry(string, string, bool) {#createentry_2}

Maakt een enkel item binnen het archief aan.

```csharp
public AppleArchiveEntry CreateEntry(string name, string path, bool openImmediately = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| pad | String | Het pad naar het te comprimeren bestand. |
| openImmediately | Boolean | True, als het bestand onmiddellijk moet worden geopend, anders wordt het bestand geopend bij het opslaan van het archief. |

### Retourwaarde

Apple Archive entry-instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Het archief is vrijgegeven. |
| ArgumentException | *name* is leeg. |
| ArgumentNullException | *path* is `null`. |

### Zie ook

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Maakt een enkel item binnen het archief aan.

```csharp
public AppleArchiveEntry CreateEntry(string name, Stream source)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| bron | Stream | De invoerstroom voor het item. |

### Retourwaarde

Apple Archive entry-instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Het archief is vrijgegeven. |
| ArgumentException | *name* is leeg. |
| ArgumentNullException | *source* is `null`. |

### Zie ook

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, bool) {#createentry}

Maakt een enkel item binnen het archief aan.

```csharp
public AppleArchiveEntry CreateEntry(string name, FileInfo fileInfo, bool openImmediately = false)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| name | String | De naam van het item. |
| fileInfo | FileInfo | De metadata van het te comprimeren bestand. |
| openImmediately | Boolean | True, als het bestand onmiddellijk moet worden geopend, anders wordt het bestand geopend bij het opslaan van het archief. |

### Retourwaarde

Apple Archive entry-instantie.

### Uitzonderingen

| uitzondering | conditie |
| --- | --- |
| ObjectDisposedException | Het archief is vrijgegeven. |
| ArgumentException | *name* is leeg. |
| ArgumentNullException | *fileInfo* is `null`. |

### Zie ook

* class [AppleArchiveEntry](../../applearchiveentry/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


