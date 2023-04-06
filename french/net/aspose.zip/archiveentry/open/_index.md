---
title: ArchiveEntry.Open
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveEntry méthode. Ouvre lentrée pour extraction et fournit un flux avec un contenu dentrée décompressé.
type: docs
weight: 110
url: /fr/net/aspose.zip/archiveentry/open/
---
## ArchiveEntry.Open method

Ouvre l'entrée pour extraction et fournit un flux avec un contenu d'entrée décompressé.

```csharp
public Stream Open(string password = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| password | String | Mot de passe facultatif pour le déchiffrement. |

### Return_Value

Le flux qui représente le contenu de l'entrée.

### Remarques

Lire à partir du flux pour obtenir le contenu original du fichier. Voir la section des exemples.

### Exemples

Utilisation :

.NET 4.0 et supérieur - utilisez la méthode Stream.CopyTo :

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 et versions antérieures - copie manuelle des octets :

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

```csharp
Stream decompressed = entry.Open();
```

### Voir également

* class [ArchiveEntry](../)
* espace de noms [Aspose.Zip](../../archiveentry/)
* Assemblée [Aspose.Zip](../../../)


