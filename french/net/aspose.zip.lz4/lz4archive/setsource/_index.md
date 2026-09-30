---
title: "Lz4Archive.SetSource"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode Lz4Archive. Définit le contenu à compresser dans l'archive"
type: docs
weight: 70
url: /fr/net/aspose.zip.lz4/lz4archive/setsource/
---
## SetSource(Stream) {#setsource_2}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(Stream source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Stream | Le flux d'entrée pour l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | L'archive est préparée pour l'extraction. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (var archive = new Lz4Archive())
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.lz4");
}
```

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource_1}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(FileInfo fileInfo)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileInfo | FileInfo | La référence à un fichier à compresser. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | L'archive est préparée pour l'extraction. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

Ouvrez une archive depuis un flux et extrayez‑la dans un `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.lz4");
}
```

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(TarArchive, TarFormat) {#setsource}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(TarArchive tarArchive, TarFormat format = TarFormat.UsTar)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| tarArchive | TarArchive | Archive Tar à compresser. |
| format | TarFormat | Définit le format d'en-tête tar. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| InvalidOperationException | Cette archive est préparée pour l'extraction. |

## Remarques

Utilisez cette méthode pour composer une archive tar.lz4 conjointe.

## Exemples

```csharp
using (var tarArchive = new TarArchive())
{
    tarArchive.CreateEntry("first.bin", "data1.bin");
    tarArchive.CreateEntry("second.bin", "data2.bin");
    using (var lz4Archive = new Lz4Archive())
    {
        lz4Archive.SetSource(tarArchive);
        lz4Archive.Save("archive.tar.lz4");
    }
}
```

### Voir aussi

* class [TarArchive](../../../aspose.zip.tar/tararchive/)
* enum [TarFormat](../../../aspose.zip.tar/tarformat/)
* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_3}

Définit le contenu à compresser dans l'archive.

```csharp
public void SetSource(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Chemin du fichier à compresser. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| InvalidOperationException | Cette archive est préparée pour l'extraction. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

Ouvrez une archive à partir d'un fichier par chemin et extrayez‑la dans un `MemoryStream`

```csharp
using (var archive = new Lz4Archive()) 
{
    archive.SetSource("data.bin");
    archive.Save("archive.lz4");
}
```

### Voir aussi

* class [Lz4Archive](../)
* namespace [Aspose.Zip.Lz4](../../lz4archive/)
* assembly [Aspose.Zip](../../../)


