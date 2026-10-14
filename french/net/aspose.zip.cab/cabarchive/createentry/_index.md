---
title: "CabArchive.CreateEntry"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode CabArchive. Crée une seule entrée dans l'archive"
type: docs
weight: 40
url: /fr/net/aspose.zip.cab/cabarchive/createentry/
---
## CreateEntry(string, string, CabEntrySettings) {#createentry_3}

Crée une seule entrée dans l'archive.

```csharp
public CabEntry CreateEntry(string name, string path, CabEntrySettings newEntrySettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| chemin | String | Le nom complet du nouveau fichier, ou le nom de fichier relatif à compresser. |
| newEntrySettings | CabEntrySettings | Paramètres de compression et de chiffrement utilisés pour l'élément [`CabEntry`](../../cabentry/) ajouté. |

### Valeur de retour

Instance d'entrée Cab.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* contient deux‑points (:) au milieu de la chaîne. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| InvalidOperationException | L'archive est préparée pour l'extraction et ne peut pas ajouter d'entrées. |

## Remarques

Le nom de l'entrée est uniquement défini dans le paramètre *name*. Le nom de fichier fourni dans le paramètre *path* n'affecte pas le nom de l'entrée.

## Exemples

```csharp
using (var archive = new CabArchive())
{
    archive.CreateEntry("entry.bin", "data.bin");
    archive.Save("archive.cab");
}
```

### Voir aussi

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream, CabEntrySettings) {#createentry_2}

Crée une seule entrée dans l'archive.

```csharp
public CabEntry CreateEntry(string name, Stream source, CabEntrySettings newEntrySettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| source | Stream | Le flux d'entrée pour l'entrée. |
| newEntrySettings | CabEntrySettings | Paramètres de compression et de chiffrement utilisés pour l'élément [`CabEntry`](../../cabentry/) ajouté. |

### Valeur de retour

Instance d'entrée Cab.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| InvalidOperationException | L'archive est préparée pour l'extraction et ne peut pas ajouter d'entrées. |
| ArgumentNullException | *name* est nul. |

## Exemples

```csharp
using (var archive = new CabArchive())
{
    using (var dataStream = new MemoryStream(File.ReadAllBytes("data.bin")))
    {
        archive.CreateEntry("stream-entry.bin", dataStream);
        archive.Save("archive.cab");
    }
}
```

```csharp
using (var archive = new CabArchive())
{     
    var settings = new CabEntrySettings(new CabStoreCompressionSettings());
    archive.CreateEntry("stream-entry.bin", dataStream, settings);
    archive.Save("archive.cab");     
}
```

### Voir aussi

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, FileInfo, CabEntrySettings) {#createentry_1}

Crée une seule entrée dans l'archive.

```csharp
public CabEntry CreateEntry(string name, FileInfo fileInfo, 
    CabEntrySettings newEntrySettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| fileInfo | FileInfo | Les métadonnées du fichier à compresser. |
| newEntrySettings | CabEntrySettings | Paramètres de compression et de chiffrement utilisés pour l'élément [`CabEntry`](../../cabentry/) ajouté. |

### Valeur de retour

Instance d'entrée CAB.

### Exceptions

| exception | condition |
| --- | --- |
| UnauthorizedAccessException | *fileInfo* est en lecture seule ou est un répertoire. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| IOException | Le fichier est déjà ouvert. |
| FileNotFoundException | *fileInfo* représente un fichier qui ne peut pas être trouvé. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder à *fileInfo*. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| InvalidOperationException | L'archive est préparée pour l'extraction et ne peut pas ajouter d'entrées. |
| ArgumentNullException | *name* est nul. |

## Remarques

Le nom de l'entrée est uniquement défini dans le paramètre *name*. Le nom de fichier fourni dans le paramètre *fileInfo* n'affecte pas le nom de l'entrée.

## Exemples

```csharp
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{
    var sourceFile = new FileInfo("logs\\log.txt");
    archive.CreateEntry("log.txt", sourceFile);
    archive.Save("archive.cab");
}
```

### Voir aussi

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Func&lt;Stream&gt;, CabEntrySettings) {#createentry}

Crée une seule entrée dans l'archive.

```csharp
public CabEntry CreateEntry(string name, Func<Stream> streamProvider, 
    CabEntrySettings newEntrySettings = null)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Le nom de l'entrée. |
| streamProvider | Func`1 | La méthode fournissant le flux d'entrée pour l'entrée. |
| newEntrySettings | CabEntrySettings | Paramètres de compression et de chiffrement utilisés pour l'élément [`CabEntry`](../../cabentry/) ajouté. |

### Valeur de retour

Instance d'entrée CAB.

### Exceptions

| exception | condition |
| --- | --- |
| InvalidOperationException | L'archive est instanciée pour la décompression. - ou - Le nombre de fichiers a atteint la limite. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentException | Le *name* est nul ou vide. |

## Exemples

```csharp
System.Func<Stream> provider = delegate(){ return new MemoryStream(new byte[]{0xFF, 0x00}); };
using (var archive = new CabArchive(new CabEntrySettings(new CabMsZipCompressionSettings())))
{    
    archive.CreateEntry("data.bin", provider);
    archive.Save("archive.cab");
}
```

### Voir aussi

* class [CabEntry](../../cabentry/)
* class [CabEntrySettings](../../cabentrysettings/)
* class [CabArchive](../)
* namespace [Aspose.Zip.Cab](../../cabarchive/)
* assembly [Aspose.Zip](../../../)


