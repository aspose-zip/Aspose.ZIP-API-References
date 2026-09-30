---
title: "WimArchive.ExtractToDirectory"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode WimArchive. Extrait l'archive vers le fichier par chemin"
type: docs
weight: 90
url: /fr/net/aspose.zip.wim/wimarchive/extracttodirectory/
---
## WimArchive.ExtractToDirectory method

Extrait l'archive vers le fichier par chemin.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | Le chemin du répertoire où placer les fichiers extraits. |

### Valeur de retour

Informations du fichier extrait.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | *destinationDirectory* est nul |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichiers moins de 260 caractères. |
| SecurityException | L’appelant ne possède pas l’autorisation requise pour accéder au répertoire existant. |
| NotSupportedException | Si le répertoire n'existe pas, le chemin contient un caractère deux-points (:) qui ne fait pas partie d'une étiquette de lecteur ("C:\\") - ou - l'archive WIM est multi-part |
| ArgumentException | le chemin est une chaîne de longueur zéro, ne contient que des espaces blancs, ou contient un ou plusieurs caractères invalides. Vous pouvez interroger les caractères invalides en utilisant la méthode System.IO.Path.GetInvalidPathChars. -ou- le chemin est préfixé ou ne contient qu'un caractère deux-points (:). |
| IOException | Le répertoire spécifié par le chemin est un fichier. -ou- Le nom du réseau est inconnu. |
| InvalidDataException | L'archive est corrompue. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |

### Voir aussi

* class [WimArchive](../)
* namespace [Aspose.Zip.Wim](../../wimarchive/)
* assembly [Aspose.Zip](../../../)


