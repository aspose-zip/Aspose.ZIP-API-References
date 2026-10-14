---
title: "ZstandardArchive.Save"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode ZstandardArchive. Enregistre l'archive dans le flux fourni"
type: docs
weight: 60
url: /fr/net/aspose.zip.zstandard/zstandardarchive/save/
---
## Save(Stream, ZstandardSaveOptions) {#save_1}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream outputStream, ZstandardSaveOptions settings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Flux de destination. |
| paramètres | ZstandardSaveOptions | Paramètres optionnels pour la composition de l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentException | *outputStream* n'est pas accessible en écriture. |
| InvalidOperationException | La source n'a pas été fournie. |

## Remarques

*outputStream* must be writable.

## Exemples

Écrire des données compressées dans le flux de réponse http.

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Voir aussi

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, ZstandardSaveOptions) {#save_2}

Enregistre l’archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, ZstandardSaveOptions settings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| paramètres | ZstandardSaveOptions | Paramètres optionnels pour la composition de l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | *destinationFileName* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *destinationFileName* est vide, ne contient que des espaces blancs, ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *destinationFileName* est refusé. |
| PathTooLongException | Le *destinationFileName* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plateformes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichiers moins de 260 caractères. |
| NotSupportedException | Le fichier à *destinationFileName* contient deux-points (:) au milieu de la chaîne. |
| Exception | Lancée lorsqu'une erreur d'exécution se produit. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, (par exemple, il se trouve sur un lecteur non mappé). |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |
| InvalidOperationException | La source n'a pas été fournie. |

## Exemples

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("result.zst");
}
```

### Voir aussi

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo, ZstandardSaveOptions) {#save}

Enregistre l’archive dans le fichier de destination fourni.

```csharp
public void Save(FileInfo destination, ZstandardSaveOptions settings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destination | FileInfo | FileInfo, qui sera ouvert en tant que flux de destination. |
| paramètres | ZstandardSaveOptions | Paramètres optionnels pour la composition de l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour ouvrir la *destination*. |
| ArgumentException | Le chemin du fichier est vide ou ne contient que des espaces. |
| FileNotFoundException | Le fichier est introuvable. |
| UnauthorizedAccessException | Le chemin vers le fichier est en lecture seule ou est un répertoire. |
| ArgumentNullException | *destination* est nul. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |
| InvalidOperationException | La source n'a pas été fournie. |

## Exemples

```csharp
using (var archive = new ZstandardArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.zst"));
}
```

### Voir aussi

* class [ZstandardSaveOptions](../../zstandardsaveoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


