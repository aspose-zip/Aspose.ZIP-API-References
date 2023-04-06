---
title: XarFileEntry.Open
second_title: Référence de l'API Aspose.ZIP pour .NET
description: XarFileEntry méthode. Ouvre lentrée pour lextraction et fournit un flux avec le contenu de lentrée.
type: docs
weight: 30
url: /fr/net/aspose.zip.xar/xarfileentry/open/
---
## XarFileEntry.Open method

Ouvre l'entrée pour l'extraction et fournit un flux avec le contenu de l'entrée.

```csharp
public abstract Stream Open()
```

### Return_Value

Le flux qui représente le contenu de l'entrée.

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

* class [XarFileEntry](../)
* espace de noms [Aspose.Zip.Xar](../../xarfileentry/)
* Assemblée [Aspose.Zip](../../../)


