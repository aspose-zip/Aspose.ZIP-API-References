---
title: SevenZipArchive.Save
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipArchive méthode. Enregistre larchive 7z dans le flux fourni.
type: docs
weight: 80
url: /fr/net/aspose.zip.sevenzip/sevenziparchive/save/
---
## Save(Stream) {#save}

Enregistre l'archive 7z dans le flux fourni.

```csharp
public void Save(Stream output)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| output | Stream | Flux de destination. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *output* ne supporte pas la recherche. |
| ArgumentNullException | *output* est nul. |
| InvalidOperationException | L'encodeur n'a pas réussi à compresser les données. |

### Remarques

*output* doit être recherchable.

### Exemples

```csharp
using (FileStream sevenZipFile = File.Open("archive.7z", FileMode.Create))
{
  using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
  {
    using (var archive = new SevenZipArchive())
    {
      archive.CreateEntry("data", source);
      archive.Save(sevenZipFile);
    }
  }
}
```

### Voir également

* class [SevenZipArchive](../)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Assemblée [Aspose.Zip](../../../)

---

## Save(string) {#save_1}

Enregistre l'archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*destinationFileName* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*destinationFileName* est refusé. |
| PathTooLongException | Le spécifié*destinationFileName*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*destinationFileName* contient deux-points (:) au milieu de la chaîne. |

### Remarques

Il est possible d'enregistrer une archive dans le même chemin que celui depuis lequel elle a été chargée. Cependant, cela n'est pas recommandé car cette approche utilise la copie dans un fichier temporaire.

### Exemples

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
   using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
   {
      archive.CreateEntry("data", source);
      archive.Save("archive.7z");
   }
}
```

### Voir également

* class [SevenZipArchive](../)
* espace de noms [Aspose.Zip.SevenZip](../../sevenziparchive/)
* Assemblée [Aspose.Zip](../../../)


