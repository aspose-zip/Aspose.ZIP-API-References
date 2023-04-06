---
title: TarArchive.SaveGzipped
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Enregistre larchive dans le flux avec compression gzip.
type: docs
weight: 130
url: /fr/net/aspose.zip.tar/tararchive/savegzipped/
---
## SaveGzipped(Stream, TarFormat?) {#savegzipped}

Enregistre l'archive dans le flux avec compression gzip.

```csharp
public void SaveGzipped(Stream output, TarFormat? format = default)
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
using (FileStream result = File.OpenWrite("result.tar.gz"))
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

## SaveGzipped(string, TarFormat?) {#savegzipped_1}

Enregistre l'archive dans le fichier par chemin avec compression gzip.

```csharp
public void SaveGzipped(string path, TarFormat? format = default)
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
        archive.SaveGzipped("result.tar.gz");
    }
}
```

### Voir également

* enum [TarFormat](../../tarformat/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


