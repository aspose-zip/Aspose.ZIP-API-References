---
title: "UueArchive.SetSource"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode UueArchive. Définit le contenu à encoder dans l'archive"
type: docs
weight: 80
url: /fr/net/aspose.zip.uue/uuearchive/setsource/
---
## SetSource(Stream) {#setsource_1}

Définit le contenu à encoder dans l'archive.

```csharp
public void SetSource(Stream source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Stream | Le flux d'entrée pour l'archive. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new MemoryStream(new byte[] { 0x00, 0xFF }));
    archive.Save("archive.uue");
}
```

### Voir aussi

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(FileInfo) {#setsource}

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
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

## Exemples

```csharp
using (var archive = new UueArchive()) 
{
    archive.SetSource(new FileInfo("data.bin"));
    archive.Save("archive.uue");
}
```

### Voir aussi

* class [UueArchive](../)
* namespace [Aspose.Zip.Uue](../../uuearchive/)
* assembly [Aspose.Zip](../../../)

---

## SetSource(string) {#setsource_2}

Définit le contenu à encoder dans l'archive.

```csharp
public void SetSource(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Chemin du fichier à encoder. |

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |

## Exemples

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


