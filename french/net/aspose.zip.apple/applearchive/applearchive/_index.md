---
title: "AppleArchive.AppleArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur AppleArchive. Initialise une nouvelle instance de la classe AppleArchive avec les paramètres utilisés pour les entrées composées."
type: docs
weight: 10
url: /fr/net/aspose.zip.apple/applearchive/applearchive/
---
## AppleArchive(AppleArchiveEntrySettings) {#constructor}

Initialise une nouvelle instance de la classe [`AppleArchive`](../) avec les paramètres utilisés pour les entrées composées.

```csharp
public AppleArchive(AppleArchiveEntrySettings newEntrySettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| newEntrySettings | AppleArchiveEntrySettings | Paramètres utilisés lors de la composition d'une nouvelle Apple Archive. |

### Voir aussi

* class [AppleArchiveEntrySettings](../../applearchiveentrysettings/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(Stream, AppleArchiveLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`AppleArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public AppleArchive(Stream sourceStream, AppleArchiveLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | La source de l'archive. |
| loadOptions | AppleArchiveLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* est nul. |
| ArgumentException | *sourceStream* n'est pas recherchable. |
| InvalidDataException | *sourceStream* n'est pas une Apple Archive valide. |
| EndOfStreamException | Le flux se termine de façon inattendue lors de l'analyse des entrées de l'archive. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir les méthodes [`ExtractToDirectory`](../extracttodirectory/) et [`Open`](../../applearchiveentry/open/) pour la décompression.

### Voir aussi

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)

---

## AppleArchive(string, AppleArchiveLoadOptions) {#constructor_2}

Initialise une nouvelle instance de la classe [`AppleArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public AppleArchive(string path, AppleArchiveLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin complet ou relatif vers le fichier d'archive. |
| loadOptions | AppleArchiveLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| FileNotFoundException | Le fichier est introuvable. |
| InvalidDataException | *path* n'est pas une Apple Archive valide. |
| EndOfStreamException | Le flux se termine de façon inattendue lors de l'analyse des entrées de l'archive. |

## Remarques

Ce constructeur ne décompresse aucune entrée. Voir les méthodes [`ExtractToDirectory`](../extracttodirectory/) et [`Open`](../../applearchiveentry/open/) pour la décompression.

### Voir aussi

* class [AppleArchiveLoadOptions](../../applearchiveloadoptions/)
* class [AppleArchive](../)
* namespace [Aspose.Zip.Apple](../../applearchive/)
* assembly [Aspose.Zip](../../../)


