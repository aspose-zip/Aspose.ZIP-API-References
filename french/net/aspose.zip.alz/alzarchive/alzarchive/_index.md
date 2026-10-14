---
title: "AlzArchive.AlzArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur AlzArchive. Initialise une nouvelle instance de la classe AlzArchive à partir d'un flux"
type: docs
weight: 10
url: /fr/net/aspose.zip.alz/alzarchive/alzarchive/
---
## AlzArchive(Stream, AlzArchiveLoadOptions) {#constructor}

Initialise une nouvelle instance de la classe [`AlzArchive`](../) à partir d'un flux.

```csharp
public AlzArchive(Stream stream, AlzArchiveLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux d'archive ALZ. Le flux doit prendre en charge la lecture et le déplacement. |
| loadOptions | AlzArchiveLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | le flux est nul. |

### Voir aussi

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)

---

## AlzArchive(string, AlzArchiveLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`AlzArchive`](../) à partir d'un chemin de fichier.

```csharp
public AlzArchive(string filePath, AlzArchiveLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| filePath | String | Chemin du fichier d'archive ALZ. |
| loadOptions | AlzArchiveLoadOptions | Options pour charger une archive existante. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | le chemin du fichier est nul. |
| FileNotFoundException | Le fichier n'existe pas. |

### Voir aussi

* class [AlzArchiveLoadOptions](../../alzarchiveloadoptions/)
* class [AlzArchive](../)
* namespace [Aspose.Zip.Alz](../../alzarchive/)
* assembly [Aspose.Zip](../../../)


