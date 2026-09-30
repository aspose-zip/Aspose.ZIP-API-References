---
title: "XzArchive.ExtractToDirectory"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode XzArchive. Extrait le contenu de l'archive vers le répertoire fourni"
type: docs
weight: 50
url: /fr/net/aspose.zip.xz/xzarchive/extracttodirectory/
---
## XzArchive.ExtractToDirectory method

Extrait le contenu de l'archive vers le répertoire fourni.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | Le chemin du répertoire où placer les fichiers extraits. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | *destinationDirectory* est nul. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichiers moins de 260 caractères. |
| SecurityException | L’appelant ne possède pas l’autorisation requise pour accéder au répertoire existant. |
| NotSupportedException | Si le répertoire n'existe pas, le chemin contient un caractère deux-points (:) qui ne fait pas partie d'une étiquette de lecteur (\"C:\\"). |
| ArgumentException | *destinationDirectory* est une chaîne de longueur zéro, ne contient que des espaces blancs, ou contient un ou plusieurs caractères invalides. Vous pouvez interroger les caractères invalides en utilisant la méthode System.IO.Path.GetInvalidPathChars. -ou- le chemin est préfixé ou ne contient que le caractère deux‑points (:). |
| IOException | Le répertoire spécifié par le chemin est un fichier. -ou- Le nom du réseau est inconnu. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |

## Remarques

Si le répertoire n’existe pas, il sera créé.

### Voir aussi

* class [XzArchive](../)
* namespace [Aspose.Zip.Xz](../../xzarchive/)
* assembly [Aspose.Zip](../../../)


