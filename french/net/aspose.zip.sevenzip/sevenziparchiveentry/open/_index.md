---
title: SevenZipArchiveEntry.Open
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipArchiveEntry méthode. Ouvre lentrée pour lextraction et fournit un flux avec le contenu de lentrée.
type: docs
weight: 90
url: /fr/net/aspose.zip.sevenzip/sevenziparchiveentry/open/
---
## SevenZipArchiveEntry.Open method

Ouvre l'entrée pour l'extraction et fournit un flux avec le contenu de l'entrée.

```csharp
public Stream Open(string password = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| password | String | Mot de passe facultatif pour le déchiffrement. |

### Return_Value

Le flux qui représente le contenu de l'entrée.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | L'archive n'est pas ouverte pour l'extraction. - ou - Cette entrée est un répertoire. |
| InvalidDataException | Données erronées dans l'entrée. |

### Remarques

Lire à partir du flux pour obtenir le contenu original du fichier. Voir la section exemples.

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

* class [SevenZipArchiveEntry](../)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchiveentry/)
* Assemblée [Aspose.Zip](../../../)


