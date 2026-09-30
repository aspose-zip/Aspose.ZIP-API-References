---
title: "LhaArchive.ExtractToDirectory"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode LhaArchive. Extrait tous les fichiers et répertoires de l'archive vers le répertoire fourni."
type: docs
weight: 40
url: /fr/net/aspose.zip.lha/lhaarchive/extracttodirectory/
---
## LhaArchive.ExtractToDirectory method

Extrait tous les fichiers et répertoires de l'archive vers le répertoire fourni.

```csharp
public void ExtractToDirectory(string destinationDirectory)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationDirectory | String | Le chemin du répertoire où placer les fichiers extraits. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationDirectory* est nul. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichiers moins de 260 caractères. |
| SecurityException | L’appelant ne possède pas l’autorisation requise pour accéder au répertoire existant. |
| NotSupportedException | Si le répertoire n'existe pas, le chemin contient un caractère deux-points (:) qui ne fait pas partie d'une étiquette de lecteur (\"C:\\"). |
| ArgumentException | *destinationDirectory* est une chaîne de longueur zéro, ne contient que des espaces blancs, ou contient un ou plusieurs caractères invalides. Vous pouvez interroger les caractères invalides en utilisant la méthode System.IO.Path.GetInvalidPathChars. -ou- le chemin est préfixé ou ne contient que le caractère deux‑points (:). |
| IOException | Le répertoire spécifié par le chemin est un fichier. -ou- Le nom du réseau est inconnu. |
| InvalidDataException | Un mot de passe incorrect a été fourni. - ou - L'archive est corrompue. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | Lancé lorsque l'objet a été libéré. |

## Remarques

Si le répertoire n’existe pas, il sera créé.

## Exemples

```csharp
using (var archive = new LhaArchive("archive.lzh")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Voir aussi

* class [LhaArchive](../)
* namespace [Aspose.Zip.Lha](../../lhaarchive/)
* assembly [Aspose.Zip](../../../)


