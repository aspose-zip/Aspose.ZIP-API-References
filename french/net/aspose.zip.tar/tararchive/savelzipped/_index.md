---
title: TarArchive.SaveLzipped
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Enregistre larchive dans le flux avec la compression lzip.
type: docs
weight: 140
url: /fr/net/aspose.zip.tar/tararchive/savelzipped/
---
## SaveLzipped(Stream, TarFormat?) {#savelzipped}

Enregistre l'archive dans le flux avec la compression lzip.

```csharp
public void SaveLzipped(Stream output, TarFormat? format = default)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| output | Stream | Flux de destination. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur nulle sera traitée comme UStar lorsque cela est possible. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* est nul. |
| ArgumentException | *output* n'est pas inscriptible. |

### Remarques

*output*doit être inscriptible.

### Exemples

```csharp
using (FileStream result = File.OpenWrite("result.tar.lz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
        }
    }
}
```

### Voir également

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## SaveLzipped(string, TarFormat?) {#savelzipped_1}

Enregistre l'archive dans le fichier par chemin avec compression lzip.

```csharp
public void SaveLzipped(string path, TarFormat? format = default)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur nulle sera traitée comme UStar lorsque cela est possible. |

### Exemples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.tar.lz");
    }
}
```

### Voir également

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


