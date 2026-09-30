---
title: "Lz4Archive.Save"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode Lz4Archive. Enregistre l'archive lz4 dans le flux fourni"
type: docs
weight: 60
url: /fr/net/aspose.zip.lz4/lz4archive/save/
---
## Save(Stream) {#save_1}

Enregistre l’archive lz4 dans le flux fourni.

```csharp
public void Save(Stream output)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | Stream | Flux de destination. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* est nul. |
| ArgumentException | *output* n'est pas accessible en écriture. |
| InvalidOperationException | L'archive est prête pour l'extraction. - ou - La source n'a pas été fournie. |
| OperationCanceledException | Dans .NET Framework 4.0 et supérieur : levée lorsque la compression est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Remarques

*output* must be seekable.

## Exemples

```csharp
using (FileStream lz4File = File.Open("archive.lz4", FileMode.Create))
{
    using (var archive = new Lz4Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(lz4File);
     }
}
```

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(FileInfo) {#save}

Enregistre l’archive lz4 dans le fichier de destination fourni.

```csharp
public void Save(FileInfo destination)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destination | FileInfo | FileInfo, qui sera ouvert en tant que flux de destination. |

### Exceptions

| exception | condition |
| --- | --- |
| SecurityException | L'appelant n'a pas l'autorisation requise pour ouvrir la *destination*. |
| ArgumentException | Le chemin du fichier est vide ou ne contient que des espaces. |
| FileNotFoundException | Le fichier est introuvable. |
| UnauthorizedAccessException | Le chemin vers le fichier est en lecture seule ou est un répertoire. |
| ArgumentNullException | *destination* est nul. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |
| InvalidOperationException | L'archive est préparée pour l'extraction. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save(new FileInfo("archive.lz4"));
}
```

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Save(string) {#save_2}

Enregistre l’archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder |
| ArgumentException | Le *destinationFileName* est vide, ne contient que des espaces blancs, ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *destinationFileName* est refusé. |
| PathTooLongException | Le *destinationFileName* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plateformes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichiers moins de 260 caractères. |
| NotSupportedException | Le fichier à *destinationFileName* contient deux-points (:) au milieu de la chaîne. |
| InvalidOperationException | L'archive est préparée pour l'extraction. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, (par exemple, il se trouve sur un lecteur non mappé). |
| FileNotFoundException | Le fichier spécifié dans *destinationFileName* est introuvable. |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |

## Exemples

```csharp
using (var archive = new LZ4Archive())
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


