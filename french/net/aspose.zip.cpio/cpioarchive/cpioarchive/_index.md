---
title: CpioArchive.CpioArchive
second_title: Référence de l'API Aspose.ZIP pour .NET
description: CpioArchive constructeur. Initialise une nouvelle instance duCpioArchive classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.cpio/cpioarchive/cpioarchive/
---
## CpioArchive() {#constructor}

Initialise une nouvelle instance du[`CpioArchive`](../) classe.

```csharp
public CpioArchive()
```

### Exemples

L'exemple suivant montre comment compresser un fichier.

```csharp
using (var archive = new CpioArchive())
{
    archive.CreateEntry("first.bin", "data.bin");
    archive.Save("archive.cpio");
}
```

### Voir également

* class [CpioArchive](../)
* espace de noms [Aspose.Zip.Cpio](../../cpioarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CpioArchive(Stream) {#constructor_1}

Initialise une nouvelle instance du[`CpioArchive`](../) la liste des entrées de classe et de composition peut être extraite de l'archive.

```csharp
public CpioArchive(Stream sourceStream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| sourceStream | Stream | La source des archives. Il doit être recherchable. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *sourceStream* est nul. |
| ArgumentException | *sourceStream* n'est pas recherchable. |
| InvalidDataException | *sourceStream* n'est pas une archive cpio valide. |

### Remarques

Ce constructeur ne décompresse aucune entrée. Voir[`Open`](../../cpioentry/open/)méthode de déballage.

### Exemples

L'exemple suivant montre comment extraire toutes les entrées d'un répertoire.

```csharp
using (var archive = new CpioArchive(File.OpenRead("archive.cpio")))
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Voir également

* class [CpioArchive](../)
* espace de noms [Aspose.Zip.Cpio](../../cpioarchive/)
* Assemblée [Aspose.Zip](../../../)

---

## CpioArchive(string) {#constructor_2}

Initialise une nouvelle instance du[`CpioArchive`](../) la liste des entrées de classe et de composition peut être extraite de l'archive.

```csharp
public CpioArchive(string path)
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

Ce constructeur ne décompresse aucune entrée. Voir[`Open`](../../cpioentry/open/)méthode de déballage.

### Exemples

L'exemple suivant montre comment extraire toutes les entrées d'un répertoire.

```csharp
using (var archive = new CpioArchive("archive.cpio")) 
{ 
   archive.ExtractToDirectory("C:\extracted");
}
```

### Voir également

* class [CpioArchive](../)
* espace de noms [Aspose.Zip.Cpio](../../cpioarchive/)
* Assemblée [Aspose.Zip](../../../)


