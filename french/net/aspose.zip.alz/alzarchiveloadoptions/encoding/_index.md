---
title: "AlzArchiveLoadOptions.Encoding"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Propriété AlzArchiveLoadOptions. Obtient ou définit l'encodage pour les noms des entrées. La valeur par défaut est la page de code Windows coréenne 949 CP949"
type: docs
weight: 40
url: /fr/net/aspose.zip.alz/alzarchiveloadoptions/encoding/
---
## AlzArchiveLoadOptions.Encoding property

Obtient ou définit l'encodage des noms des entrées. La valeur par défaut est la page de code Windows coréenne 949 (CP949).

```csharp
public Encoding Encoding { get; set; }
```

## Remarques

Les archives ALZ stockent historiquement les noms de fichiers en utilisant la page de code ANSI Windows coréenne.

## Exemples

Nom d'entrée composé en utilisant l'encodage spécifié.

```csharp
using (FileStream fs = File.OpenRead("archive.alz"))
{
    using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { Encoding = System.Text.Encoding.GetEncoding(949) }))
    {
        string name = archive.Entries[0].Name;
    }
}
```

### Voir aussi

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


