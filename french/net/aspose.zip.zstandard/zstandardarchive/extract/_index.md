---
title: "ZstandardArchive.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode ZstandardArchive. Extrait l'archive dans le flux fourni"
type: docs
weight: 30
url: /fr/net/aspose.zip.zstandard/zstandardarchive/extract/
---
## Extract(Stream) {#extract_1}

Extrait l'archive vers le flux fourni.

```csharp
public void Extract(Stream destination)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être accessible en écriture. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentException | *destination* ne prend pas en charge l'écriture. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |

## Exemples

```csharp
using (var archive = new GzipArchive("archive.zst"))
{
     archive.Extract(httpResponseStream);
}
```

### Voir aussi

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## Extract(string) {#extract}

Extrait l'archive vers le fichier par chemin.

```csharp
public FileInfo Extract(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

### Valeur de retour

Info d'un fichier extrait.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |

### Voir aussi

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


