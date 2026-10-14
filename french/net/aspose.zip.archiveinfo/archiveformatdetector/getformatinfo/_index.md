---
title: "GetFormatInfo"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: 
type: docs
weight: 20
url: /fr/net/aspose.zip.archiveinfo/archiveformatdetector/getformatinfo/
---
## ArchiveFormatDetector.GetFormatInfo method (1 of 2)

Obtient les informations de format.

```csharp
public ArchiveFormatInfo GetFormatInfo(string fileName)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| fileName | String | Le nom de fichier de l'archive. |

### Valeur de retour

Informations sur le format d'archive ou null si le format n'a pas été détecté.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *fileName* est nul. |
| SecurityException | L'appelant ne possède pas l'autorisation requise pour accéder. |
| ArgumentException | Le *fileName* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *fileName* est refusé. |
| PathTooLongException | Le *fileName* spécifié dépasse la longueur maximale définie par le système. Par exemple, sur les plateformes Windows, les chemins doivent être inférieurs à 248 caractères et les noms de fichiers à 260 caractères. |
| NotSupportedException | Le fichier à *fileName* contient deux-points (:) au milieu de la chaîne. |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |

### Voir aussi

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

---

## ArchiveFormatDetector.GetFormatInfo method (2 of 2)

Obtient les informations de format.

```csharp
public ArchiveFormatInfo GetFormatInfo(Stream stream)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| stream | Stream | Le flux du fichier d'archive. |

### Valeur de retour

Informations sur le format d'archive ou null si le format n'a pas été détecté.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* est nul. |
| ArgumentException | *stream* n'est pas recherchable. |

### Voir aussi

* class [ArchiveFormatInfo](../../archiveformatinfo)
* class [ArchiveFormatDetector](../../archiveformatdetector)
* namespace [Aspose.Zip.ArchiveInfo](../../archiveformatdetector)
* assembly [Aspose.Zip](../../../)

<!-- NE PAS MODIFIER : généré par xmldocmd pour Aspose.Zip.dll -->
