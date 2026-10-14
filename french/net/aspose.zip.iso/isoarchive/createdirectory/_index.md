---
title: "IsoArchive.CreateDirectory"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode IsoArchive. Ajoute un répertoire à l'image ISO"
type: docs
weight: 30
url: /fr/net/aspose.zip.iso/isoarchive/createdirectory/
---
## IsoArchive.CreateDirectory method

Ajoute un répertoire à l'image ISO.

```csharp
public IsoEntry CreateDirectory(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Chemin du répertoire dans l'ISO. |

### Valeur de retour

L'entrée ISO composée.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | L'archive est ouverte pour l'extraction. |
| ArgumentNullException | `name` est nul ou vide. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

### Voir aussi

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


