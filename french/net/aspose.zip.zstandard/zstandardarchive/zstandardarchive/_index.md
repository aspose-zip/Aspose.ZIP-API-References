---
title: "ZstandardArchive.ZstandardArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur ZstandardArchive. Initialise une nouvelle instance de la classe ZstandardArchive préparée pour la compression"
type: docs
weight: 10
url: /fr/net/aspose.zip.zstandard/zstandardarchive/zstandardarchive/
---
## ZstandardArchive() {#constructor}

Initialise une nouvelle instance de la classe [`ZstandardArchive`](../) préparée pour la compression.

```csharp
public ZstandardArchive()
```

## Exemples

L'exemple suivant montre comment compresser un fichier.

```csharp
using (ZstandardArchive archive = new ZstandardArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.zst");
}
```

### Voir aussi

* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(Stream, ZstandardLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`ZstandardArchive`](../) préparée pour la décompression.

```csharp
public ZstandardArchive(Stream sourceStream, ZstandardLoadOptions options = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | La source de l'archive. |
| options | ZstandardLoadOptions | Les options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| EndOfStreamException | Lancée lorsque la fin du flux est atteinte de manière inattendue. |
| IOException | Une erreur d'E/S se produit. |
| InvalidDataException | Lancé lorsque les données sont invalides ou corrompues. |

## Remarques

Ce constructeur ne décompresse pas. Voir la méthode [`Open`](../open/) pour la décompression.

## Exemples

Ouvrez une archive depuis un flux et extrayez‑la dans un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (GzipArchive archive = new ZstandardArchive(File.OpenRead("archive.zst")))
  archive.Open().CopyTo(ms);
```

### Voir aussi

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)

---

## ZstandardArchive(string, ZstandardLoadOptions) {#constructor_2}

Initialise une nouvelle instance de la classe [`ZstandardArchive`](../).

```csharp
public ZstandardArchive(string path, ZstandardLoadOptions options = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin vers le fichier d'archive. |
| options | ZstandardLoadOptions | Les options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| EndOfStreamException | Lancée lorsque la fin du flux est atteinte de manière inattendue. |
| FileNotFoundException | Le fichier est introuvable. |
| IOException | Le fichier est déjà ouvert. |
| InvalidDataException | Lancé lorsque les données sont invalides ou corrompues. |

## Remarques

Ce constructeur ne décompresse pas. Voir la méthode [`Open`](../open/) pour la décompression.

## Exemples

Ouvrez une archive à partir d'un fichier par chemin et extrayez‑la dans un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (ZstandardArchive archive = new ZstandardArchive("archive.zst"))
  archive.Open().CopyTo(ms);
```

### Voir aussi

* class [ZstandardLoadOptions](../../zstandardloadoptions/)
* class [ZstandardArchive](../)
* namespace [Aspose.Zip.Zstandard](../../zstandardarchive/)
* assembly [Aspose.Zip](../../../)


