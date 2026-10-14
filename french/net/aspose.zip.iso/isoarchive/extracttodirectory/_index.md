---
title: "IsoArchive.ExtractToDirectory"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode IsoArchive. Extrait toutes les entrées vers le répertoire spécifié"
type: docs
weight: 60
url: /fr/net/aspose.zip.iso/isoarchive/extracttodirectory/
---
## IsoArchive.ExtractToDirectory method

Extrait toutes les entrées vers le répertoire spécifié.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | Le répertoire où extraire les entrées. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Lancée lorsque l'archive est en mode édition. |
| ArgumentNullException | Lancée lorsque le *destinationDirectory* est nul. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

L'exemple suivant montre comment extraire toutes les entrées vers un répertoire :

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Voir aussi

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


