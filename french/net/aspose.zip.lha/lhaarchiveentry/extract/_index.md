---
title: "LhaArchiveEntry.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode LhaArchiveEntry. Extrait l'entrée d'archive Lha vers un système de fichiers par chemin"
type: docs
weight: 60
url: /fr/net/aspose.zip.lha/lhaarchiveentry/extract/
---
## Extract(string) {#extract}

Extrait l'entrée d'archive Lha vers un système de fichiers par chemin.

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
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| InvalidDataException | Lancé lorsque les données sont invalides ou corrompues. |

## Exemples

```csharp
using (FileStream lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract("extracted.bin");
    }
}
```

### Voir aussi

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_2}

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
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| InvalidDataException | Lancé lorsque les données sont invalides ou corrompues. |

## Remarques

Ne fait rien pour l'entrée de répertoire.

### Voir aussi

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrait l'entrée d'archive Lha vers un fichier.

```csharp
public void Extract(FileInfo fileInfo)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileInfo | FileInfo | FileInfo pour stocker les données décompressées. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | Les en-têtes d'archive et les informations de service n'ont pas été lus. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour ouvrir le *fileInfo*. |
| ArgumentException | Le chemin du fichier est vide ou ne contient que des espaces. |
| FileNotFoundException | Le fichier est introuvable. |
| UnauthorizedAccessException | Le chemin vers le fichier est en lecture seule ou est un répertoire. |
| ArgumentNullException | *fileInfo* est nul. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |

## Remarques

Ne fait rien pour l'entrée de répertoire.

## Exemples

```csharp
using (var lhaFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new LhaArchive(lhaFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Voir aussi

* class [LhaArchiveEntry](../)
* namespace [Aspose.Zip.Lha](../../lhaarchiveentry/)
* assembly [Aspose.Zip](../../../)


