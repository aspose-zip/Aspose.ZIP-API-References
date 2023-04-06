---
title: Bzip2Archive.SetSource
second_title: Référence de l'API Aspose.ZIP pour .NET
description: Bzip2Archive méthode. Définit le contenu à compresser dans larchive.
type: docs
weight: 60
url: /fr/net/aspose.zip.bzip2/bzip2archive/setsource/
---
## SetSource(Stream) {#setsource_3}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(Stream source)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| source | Stream | Le flux d'entrée pour l'archive. |

### Exemples

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00,0xFF }));
    archive.Save("archive.bz2");
}
```

### Voir également

* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_2}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileInfo | FileInfo | La référence à un fichier à compresser. |

### Exemples

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.bz2");
}
```

### Voir également

* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_4}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier à compresser. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*path* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*path* est refusé. |
| PathTooLongException | Le spécifié*path*, nom de fichier ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*path* contient deux-points (:) au milieu de la chaîne. |

### Exemples

```csharp
using (Bzip2Archive archive = new Bzip2Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.bz2");
}
```

### Voir également

* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource_1}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| tarArchive | TarArchive | Archive tar à compresser. |
| format | TarFormat | Définit le format d'en-tête tar. |

### Remarques

Utilisez cette méthode pour composer une archive tar.bz2 conjointe.

### Exemples

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(tarArchive);
        bzippedArchive.Save("archive.tar.bz2");
    }
}
```

### Voir également

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)

---

## SetSource(CpioArchive, CpioFormat) {#setsource}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(CpioArchive cpioArchive, CpioFormat format = CpioFormat.OldAscii)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| cpioArchive | CpioArchive | Archive cpio à compresser. |
| format | CpioFormat | Définit le format d'en-tête cpio. |

### Remarques

Utilisez cette méthode pour composer une archive commune cpio.bz2.

### Exemples

```csharp
using (var cpioArchive = new CpioArchive())
{
    cpioArchive.CreateEntry("first.bin", "data1.bin");
    cpioArchive.CreateEntry("second.bin", "data2.bin");
    using (var bzippedArchive = new Bzip2Archive())
    {
        bzippedArchive.SetSource(cpioArchive);
        bzippedArchive.Save("archive.cpio.bz2");
    }
}
```

### Voir également

* class [CpioArchive](../../../aspose.zip.cpio/cpioarchive/)
* enum [CpioFormat](../../../aspose.zip.cpio/cpioformat/)
* class [Bzip2Archive](../)
* espace de noms [Aspose.Zip.Bzip2](../../bzip2archive/)
* Assemblée [Aspose.Zip](../../../)


