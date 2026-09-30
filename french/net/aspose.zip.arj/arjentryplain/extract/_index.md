---
title: "ArjEntryPlain.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode ArjEntryPlain. Extrait l'entrée dans le système de fichiers selon le chemin fourni"
type: docs
weight: 40
url: /fr/net/aspose.zip.arj/arjentryplain/extract/
---
## Extract(string) {#extract}

Extrait l'entrée dans le système de fichiers au chemin fourni.

```csharp
public FileInfo Extract(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

### Valeur de retour

Les informations du fichier d'un fichier composé.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul ou vide. |
| ObjectDisposedException | Lancée si l'archive a été libérée. |
| FileNotFoundException | Le fichier est introuvable. |
| InvalidDataException | Incohérence de la somme de contrôle pour les en‑têtes ou les données. - ou - L’archive est corrompue. |
| PathTooLongException | Le chemin spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. |
| NotImplementedException | Entrée compressée avec la méthode 4. |

## Exemples

Extraire deux entrées d'une archive rar.

```csharp
using (FileStream arjFile = File.Open("archive.arj", FileMode.Open))
{
    using (ArjArchive archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract("first.bin");
        archive.Entries[1].Extract("second.bin");
    }
}
```

### Voir aussi

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)

---

## Extract(FileInfo) {#extract_1}

Extrait l'entrée d'archive ARJ vers un fichier.

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
| ObjectDisposedException | Lancée si l'archive a été libérée. |
| InvalidDataException | Incohérence de la somme de contrôle pour les en‑têtes ou les données. - ou - L’archive est corrompue. |
| NotImplementedException | Entrée compressée avec la méthode 4. |

## Exemples

```csharp
using (var arjFile = File.Open(sourceFileName, FileMode.Open))
{
    using (var archive = new ArjArchive(arjFile))
    {
        archive.Entries[0].Extract(new FileInfo("extracted.bin"));
    }
}
```

### Voir aussi

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
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
| InvalidDataException | Incohérence de la somme de contrôle pour les en‑têtes ou les données. - ou - L’archive est corrompue. |
| NotImplementedException | Entrée compressée avec la méthode 4. |
| OperationCanceledException | Dans .NET Framework 4.0 et versions ultérieures : Lancée lorsque l'extraction est annulée via le jeton d'annulation fourni. |
| ObjectDisposedException | Lancée si l'archive a été libérée. |

### Voir aussi

* class [ArjEntryPlain](../)
* namespace [Aspose.Zip.Arj](../../arjentryplain/)
* assembly [Aspose.Zip](../../../)


