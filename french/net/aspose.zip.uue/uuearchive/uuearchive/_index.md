---
title: "UueArchive.UueArchive"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Constructeur UueArchive. Initialise une nouvelle instance de la classe UueArchive préparée pour l'encodage."
type: docs
weight: 10
url: /fr/net/aspose.zip.uue/uuearchive/uuearchive/
---
## UueArchive() {#constructor}

Initialise une nouvelle instance de la classe [`UueArchive`](../) préparée pour l'encodage.

```csharp
public UueArchive()
```

## Exemples

L'exemple suivant montre comment uuencoder un fichier.

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.uue");
}
```

### Voir aussi

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(Stream) {#constructor_1}

Initialise une nouvelle instance de la classe [`UueArchive`](../) préparée pour le décodage.

```csharp
public UueArchive(Stream sourceStream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| sourceStream | Stream | La source de l'archive. |

## Remarques

Ce constructeur ne décode pas. Voir la méthode [`Open`](../open/) pour la décompression.

## Exemples

Ouvrez une archive depuis un flux et extrayez‑la dans un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive(File.OpenRead("archive.001")))
  archive.Open().CopyTo(ms);
```

### Voir aussi

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## UueArchive(string) {#constructor_2}

Initialise une nouvelle instance de la classe [`UueArchive`](../).

```csharp
public UueArchive(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin vers le fichier d'archive. |

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
| FileNotFoundException | Le fichier est introuvable. |
| IOException | Le fichier est déjà ouvert. |

## Remarques

Ce constructeur ne décompresse pas. Voir la méthode [`Open`](../open/) pour la décompression.

## Exemples

Ouvrir une archive depuis un fichier par chemin et la décoder en un `MemoryStream`

```csharp
var ms = new MemoryStream();
using (var archive = new UueArchive("archive.uue"))
  archive.Open().CopyTo(ms);
```

### Voir aussi

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)


