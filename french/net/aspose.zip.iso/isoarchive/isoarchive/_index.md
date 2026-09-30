---
title: "IsoArchive.IsoArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur IsoArchive. Initialise une nouvelle instance de la classe IsoArchive et crée une archive ISO vide pour ajouter de nouveaux fichiers et répertoires."
type: docs
weight: 10
url: /fr/net/aspose.zip.iso/isoarchive/isoarchive/
---
## IsoArchive() {#constructor}

Initialise une nouvelle instance de la classe [`IsoArchive`](../) et crée une archive ISO vide pour ajouter de nouveaux fichiers et répertoires.

```csharp
public IsoArchive()
```

## Exemples

L'exemple suivant montre comment créer une nouvelle archive ISO vide et y ajouter des fichiers :

```csharp
// Créer une nouvelle archive ISO vide
using(IsoArchive isoArchive = new IsoArchive())
{
    // Ajouter des fichiers à l'archive ISO
    isoArchive.CreateEntry("example_file.txt", "path_to_file.txt");

    // Enregistrer l'archive ISO dans un fichier
    isoArchive.Save("new_archive.iso");
}
```

### Voir aussi

* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(Stream, IsoLoadOptions) {#constructor_1}

Initialise une nouvelle instance de la classe [`IsoArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public IsoArchive(Stream sourceStream, IsoLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | La source de l'archive. Elle doit être recherchable. |
| loadOptions | IsoLoadOptions | Les options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* est nul. |
| ArgumentException | *sourceStream* n'est pas recherchable. |
| InvalidDataException | *sourceStream* n'est pas une archive ISO valide. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| EndOfStreamException | Lancée lorsque la fin du flux est atteinte de manière inattendue. |
| IOException | Une erreur d'E/S se produit. |
| NotSupportedException | Le flux ne prend pas en charge la lecture. |

## Remarques

Ce constructeur ne décompresse aucune entrée.

## Exemples

L'exemple suivant montre comment extraire toutes les entrées vers un répertoire.

```csharp
using (var archive = new IsoArchive(File.OpenRead("archive.iso")))
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Voir aussi

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## IsoArchive(string, IsoLoadOptions) {#constructor_2}

Initialise une nouvelle instance de la classe [`IsoArchive`](../) et compose une liste d'entrées pouvant être extraites de l'archive.

```csharp
public IsoArchive(string path, IsoLoadOptions loadOptions = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin vers le fichier d'archive. |
| loadOptions | IsoLoadOptions | Les options pour charger l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| FileNotFoundException | Le fichier est introuvable. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |
| EndOfStreamException | Le fichier est trop court. |
| InvalidDataException | Lancé lorsque les données sont invalides ou corrompues. |

## Remarques

Ce constructeur ne décompresse aucune entrée.

## Exemples

L'exemple suivant montre comment extraire toutes les entrées vers un répertoire.

```csharp
using (var archive = new IsoArchive("archive.iso")) 
{ 
   archive.ExtractToDirectory("C:\\extracted");
}
```

### Voir aussi

* class [IsoLoadOptions](../../isoloadoptions/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


