---
title: SharArchive.SharArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SharArchive constructeur. Initialise une nouvelle instance duSharArchive classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.shar/shararchive/shararchive/
---
## SharArchive() {#constructor}

Initialise une nouvelle instance du[`SharArchive`](../) classe.

```csharp
public SharArchive()
```

### Exemples

L'exemple suivant montre comment compresser un fichier.

```csharp
using (var archive = new SharArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.shar");
}
```

### Voir également

* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## SharArchive(string) {#constructor_1}

```csharp
public SharArchive(string path)
```

### Voir également

* class [SharArchive](../)
* espace de noms [Aspose.Zip.Shar](../../shararchive/)
* Assemblée [Aspose.Zip](../../../)


