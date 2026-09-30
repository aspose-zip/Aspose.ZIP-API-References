---
title: "ArjArchive.ExtractToDirectory"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode ArjArchive. Extrait toutes les entrées vers le répertoire spécifié"
type: docs
weight: 60
url: /fr/net/aspose.zip.arj/arjarchive/extracttodirectory/
---
## ArjArchive.ExtractToDirectory method

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
| ArgumentNullException | Lancée lorsque le *destinationDirectory* est nul. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| InvalidDataException | Incohérence de la somme de contrôle pour les en‑têtes ou les données. - ou - L’archive est corrompue. |
| NotImplementedException | Entrée compressée avec la méthode 4. |

## Exemples

L'exemple suivant montre comment extraire toutes les entrées vers un répertoire :

```csharp
using (var archive = new ArjArchive(File.OpenRead("archive.arj")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Voir aussi

* class [ArjArchive](../)
* namespace [Aspose.Zip.Arj](../../arjarchive/)
* assembly [Aspose.Zip](../../../)


