---
title: "XarArchive.Save"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode XarArchive. Enregistre l'archive dans le fichier de destination fourni"
type: docs
weight: 80
url: /fr/net/aspose.zip.xar/xararchive/save/
---
## Save(string, XarSaveOptions) {#save_1}

Enregistre l’archive dans le fichier de destination fourni.

```csharp
public void Save(string destinationFileName, XarSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destinationFileName | String | Le chemin de l'archive à créer. Si le nom de fichier spécifié pointe vers un fichier existant, il sera écrasé. |
| saveOptions | XarSaveOptions | Options pour enregistrer l'archive xar. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *destinationFileName* est nul. |
| InvalidOperationException | Impossible de modifier l'archive xar. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. |
| UnauthorizedAccessException | *destinationFileName* spécifie un fichier en lecture seule. -ou- *destinationFileName* spécifie un répertoire. -ou- L'appelant ne possède pas l'autorisation requise. |

### Voir aussi

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)

---

## Save(Stream, XarSaveOptions) {#save}

Enregistre l'archive dans le flux fourni.

```csharp
public void Save(Stream output, XarSaveOptions saveOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sortie | Stream | Flux de destination. |
| saveOptions | XarSaveOptions | Options pour enregistrer l'archive xar. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *output* est nul. |
| ArgumentException | *output* n'est pas inscriptible/consultable ou n'est pas positionnable. |
| InvalidOperationException | Impossible de modifier l'archive xar. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

### Voir aussi

* class [XarSaveOptions](../../xarsaveoptions/)
* class [XarArchive](../)
* namespace [Aspose.Zip.Xar](../../xararchive/)
* assembly [Aspose.Zip](../../../)


