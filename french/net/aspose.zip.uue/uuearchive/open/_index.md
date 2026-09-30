---
title: "UueArchive.Open"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode UueArchive. Ouvre l'archive pour le décodage et fournit un flux contenant le contenu de l'archive"
type: docs
weight: 60
url: /fr/net/aspose.zip.uue/uuearchive/open/
---
## UueArchive.Open method

Ouvre l'archive pour le décodage et fournit un flux contenant le contenu de l'archive.

```csharp
public Stream Open()
```

### Valeur de retour

Le flux qui représente le contenu de l'archive.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

Lisez le flux pour obtenir le contenu original d'un fichier. Voir la section des exemples.

## Exemples

Utilisation:

```csharp
Stream decompressed = archive.Open();
```

.NET 4.0 et supérieur - utilisez la méthode Stream.CopyTo :

```csharp
decompressed.CopyTo(httpResponse.OutputStream)
```

.NET 3.5 et antérieur - copiez les octets manuellement :

```csharp
byte[] buffer = new byte[8192];
int bytesRead;
while (0 < (bytesRead = decompressed.Read(buffer, 0, buffer.Length)))
 fileStream.Write(buffer, 0, bytesRead);
```

### Voir aussi

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


