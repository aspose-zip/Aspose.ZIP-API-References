---
title: "UueArchive.Save"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode UueArchive. Enregistre l'archive dans le flux fourni"
type: docs
weight: 70
url: /fr/net/aspose.zip.uue/uuearchive/save/
---
## Save(Stream, UueSaveOptions) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream outputStream, UueSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| outputStream | Stream | Flux de destination. |
| saveOptions | UueSaveOptions | Options pour l'enregistrement de l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| InvalidOperationException | La source des données à archiver n'a pas été fournie. |
| ArgumentException | *outputStream* n'est pas accessible en écriture. |
| UnauthorizedAccessException | La source du fichier est en lecture seule ou est un répertoire. |
| DirectoryNotFoundException | Le chemin de la source de fichier spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | La source du fichier est déjà ouverte. |

## Remarques

*outputStream* must be writable.

## Exemples

Écrire des données compressées dans le flux de réponse http.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(httpResponse.OutputStream);
}
```

### Voir aussi

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string, UueSaveOptions) {#save_1}

Enregistre l'archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, UueSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| saveOptions | UueSaveOptions | Options pour l'enregistrement de l'archive. |

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
| InvalidOperationException | La source des données à archiver n'a pas été fournie. |

## Exemples

Écrire des données encodées dans le fichier.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("data.uue");
}
```

### Voir aussi

* class [UueSaveOptions](../../uuesaveoptions/)
* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


