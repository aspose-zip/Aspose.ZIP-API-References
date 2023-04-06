---
title: TarArchive.SaveXzCompressed
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Enregistre larchive dans le flux avec une compression xz.
type: docs
weight: 150
url: /fr/net/aspose.zip.tar/tararchive/savexzcompressed/
---
## SaveXzCompressed(Stream, TarFormat?, XzArchiveSettings) {#savexzcompressed}

Enregistre l'archive dans le flux avec une compression xz.

```csharp
public void SaveXzCompressed(Stream output, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| output | Stream | Flux de destination. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur nulle sera traitée comme UStar lorsque cela est possible. |
| settings | XzArchiveSettings | Ensemble de paramètres d'archive xz particuliers : taille du dictionnaire, taille du bloc, type de contrôle. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* est nul. |
| ArgumentException | *output* n'est pas inscriptible. |

### Remarques

*output*Le flux doit être accessible en écriture.

### Exemples

```csharp
using (FileStream result = File.OpenWrite("result.tar.xz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new TarArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveXzCompressed(result);
        }
    }
}
```

### Voir également

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## SaveXzCompressed(string, TarFormat?, XzArchiveSettings) {#savexzcompressed_1}

Enregistre l'archive dans le chemin par chemin avec une compression xz.

```csharp
public void SaveXzCompressed(string path, TarFormat? format = default, 
    XzArchiveSettings settings = null)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| format | Nullable`1 | Définit le format d'en-tête tar. La valeur nulle sera traitée comme UStar lorsque cela est possible. |
| settings | XzArchiveSettings | Ensemble de paramètres d'archive xz particuliers : taille du dictionnaire, taille du bloc, type de contrôle. |

### Exemples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new TarArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveXzCompressed("result.tar.xz");
    }
}
```

### Voir également

* enum [TarFormat](../../tarformat/)
* class [XzArchiveSettings](../../../aspose.zip.xz.settings/xzarchivesettings/)
* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


