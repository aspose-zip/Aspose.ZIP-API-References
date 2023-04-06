---
title: Bzip2Archive.Extract
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Bzip2Archive méthode. Extrait larchive dans le flux fourni.
type: docs
weight: 30
url: /fr/net/aspose.zip.bzip2/bzip2archive/extract/
---
## Bzip2Archive.Extract method

Extrait l'archive dans le flux fourni.

```csharp
public void Extract(Stream destination)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être inscriptible. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* ne prend pas en charge l'écriture. |

### Exemples

```csharp
using (Bzip2Archive archive = new Bzip2Archive("archive.bz2"))
{
     archive.Extract(httpResponseStream);
}
```

### Voir également

* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)


