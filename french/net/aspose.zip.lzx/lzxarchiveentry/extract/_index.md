---
title: "LzxArchiveEntry.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode LzxArchiveEntry. Extrait l'entrée d'archive Lzx vers un système de fichiers par chemin"
type: docs
weight: 80
url: /fr/net/aspose.zip.lzx/lzxarchiveentry/extract/
---
## Extract(string) {#extract}

Extrait l'entrée d'archive Lzx vers un système de fichiers par chemin.

```csharp
public FileSystemInfo Extract(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Chemin du fichier qui stockera les données décompressées. |

### Valeur de retour

FileSystemInfoInstance contenant les données extraites.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Les en-têtes d'archive et les informations de service n'ont pas été lus. |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| InvalidDataException | Incohérence de la somme de contrôle pour les en‑têtes ou les données. - ou - L’archive est corrompue. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| NotSupportedException | Méthode de compression invalide. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| EndOfStreamException | Lancée lorsque la fin du flux est atteinte de manière inattendue. |

## Exemples

```csharp
using (FileStream lzxFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LzxArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Voir aussi

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrait l'entrée vers le flux fourni.

```csharp
public void Extract(Stream destination)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être accessible en écriture. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | *destination* ne prend pas en charge l'écriture. |
| InvalidDataException | Incohérence de la somme de contrôle pour les en‑têtes ou les données. - ou - L’archive est corrompue. |
| ArgumentNullException | Le flux de destination est nul. |
| NotSupportedException | Méthode de compression invalide. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| EndOfStreamException | Lancée lorsque la fin du flux est atteinte de manière inattendue. |

### Voir aussi

* class [LzxArchiveEntry](../)
* namespace [Aspose.Zip.Lzx](../../lzxarchiveentry/)
* assembly [Aspose.Zip](../../../)


