---
title: "Lz4Archive.Lz4Archive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur Lz4Archive. Initialise une nouvelle instance de la classe Lz4Archive préparée pour la décompression"
type: docs
weight: 10
url: /fr/net/aspose.zip.lz4/lz4archive/lz4archive/
---
## Lz4Archive(Stream, Lz4LoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`Lz4Archive`](../) préparée pour la décompression.

```csharp
public Lz4Archive(Stream sourceStream, Lz4LoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | La source de l'archive. |
| loadOptions | Lz4LoadOptions | Les options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Impossible de lire depuis *sourceStream* |
| ArgumentNullException | *sourceStream* est nul. |
| EndOfStreamException | *sourceStream* est trop court. |
| InvalidDataException | Le *sourceStream* a une signature incorrecte. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| IOException | Une erreur d'E/S se produit. |

## Remarques

Ce constructeur ne décompresse pas. Voir la méthode [`Open`](../open/) pour la décompression.

## Exemples

Ouvrez une archive depuis un flux et extrayez‑la dans un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive(File.OpenRead("archive.lz4")))
  archive.Open().CopyTo(ms);
```

### Voir aussi

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(string, Lz4LoadOptions) {#constructor_2}

Initialise une nouvelle instance de la classe [`Lz4Archive`](../).

```csharp
public Lz4Archive(string path, Lz4LoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin vers le fichier d'archive. |
| loadOptions | Lz4LoadOptions | Les options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| EndOfStreamException | Le fichier est trop court. |
| InvalidDataException | Les données du fichier ont une signature incorrecte. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| FileNotFoundException | Le fichier est introuvable. |
| IOException | Le fichier est déjà ouvert. |

## Remarques

Ce constructeur ne décompresse pas. Voir la méthode [`Open`](../open/) pour la décompression.

## Exemples

Ouvrez une archive à partir d'un fichier par chemin et extrayez‑la dans un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (Lz4Archive archive = new Lz4Archive("archive.lz4"))
  archive.Open().CopyTo(ms);
```

### Voir aussi

* class [Lz4LoadOptions](../../lz4loadoptions/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## Lz4Archive(Lz4ArchiveSetting) {#constructor}

Initialise une nouvelle instance de la classe [`Lz4Archive`](../) préparée pour la compression.

```csharp
public Lz4Archive(Lz4ArchiveSetting settings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| paramètres | Lz4ArchiveSetting | Le paramètre de l'archive composée. |

### Voir aussi

* class [Lz4ArchiveSetting](../../lz4archivesetting/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


