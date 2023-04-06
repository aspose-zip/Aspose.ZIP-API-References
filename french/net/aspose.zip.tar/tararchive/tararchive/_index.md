---
title: TarArchive.TarArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive constructeur. Initialise une nouvelle instance duTarArchive classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.tar/tararchive/tararchive/
---
## TarArchive() {#constructor}

Initialise une nouvelle instance du[`TarArchive`](../) classe.

```csharp
public TarArchive()
```

### Exemples

L'exemple suivant montre comment compresser un fichier.

```csharp
using (var archive = new TarArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.tar");
}
```

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## TarArchive(Stream) {#constructor_1}

Initialise une nouvelle instance du[`Archive`](../../../aspose.zip/archive/) la liste des entrées de classe et de composition peut être extraite de l'archive.

```csharp
public TarArchive(Stream sourceStream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceStream | Stream | La source des archives. Il doit être recherchable. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | *sourceStream* n'est pas recherchable. |

### Remarques

Ce constructeur ne décompresse aucune entrée. Voir[`Open`](../../tarentry/open/)méthode de déballage.

### Exemples

L'exemple suivant montre comment extraire toutes les entrées d'un répertoire.

```csharp
using (var archive = new TarArchive(File.OpenRead("archive.tar")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## TarArchive(string) {#constructor_2}

Initialise une nouvelle instance du[`TarArchive`](../) la liste des entrées de classe et de composition peut être extraite de l'archive.

```csharp
public TarArchive(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier d'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*path* est refusé. |
| PathTooLongException | Le spécifié*path*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*path* contient deux-points (:) au milieu de la chaîne. |

### Remarques

Ce constructeur ne décompresse aucune entrée. Voir[`Open`](../../tarentry/open/)méthode de déballage.

### Exemples

L'exemple suivant montre comment extraire toutes les entrées d'un répertoire.

```csharp
using (var archive = new TarArchive("archive.tar")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


