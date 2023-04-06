---
title: ArchiveInstanceInfo.GetArchiveInstanceInfo
second_title: Référence de l'API Aspose.ZIP pour .NET
description: ArchiveInstanceInfo méthode. Obtient les informations sur linstance darchive.
type: docs
weight: 10
url: /fr/net/aspose.zip.archiveinfo/archiveinstanceinfo/getarchiveinstanceinfo/
---
## GetArchiveInstanceInfo(string) {#getarchiveinstanceinfo_1}

Obtient les informations sur l'instance d'archive.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(string fileName)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| fileName | String | Le nom de fichier du fichier d'archive. |

### Return_Value

Informations sur l'instance d'archive ou null si le format n'a pas été détecté.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *fileName* est nul. |
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder. |
| ArgumentException | Le*fileName* est vide, ne contient que des espaces blancs ou contient des caractères non valides. |
| UnauthorizedAccessException | Accéder au dossier*fileName* est refusé. |
| PathTooLongException | Le spécifié*fileName* dépasse la longueur maximale définie par le système. Par exemple, sur les plates-formes Windows, les chemins doivent comporter moins de 248 caractères et les noms de fichiers doivent comporter moins de 260 caractères. |
| NotSupportedException | Fichier à*fileName* contient deux-points (:) au milieu de la chaîne. |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |

### Voir également

* class [ArchiveInstanceInfo](../)
* espace de noms [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* Assemblée [Aspose.Zip](../../../)

---

## GetArchiveInstanceInfo(Stream) {#getarchiveinstanceinfo}

Obtient les informations sur l'instance d'archive.

```csharp
public static ArchiveInstanceInfo GetArchiveInstanceInfo(Stream stream)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| stream | Stream | Le flux du fichier d'archive. |

### Return_Value

Informations sur l'instance d'archive ou null si le format n'a pas été détecté.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *stream* est nul. |
| ArgumentException | *stream* n'est pas recherchable. |

### Voir également

* class [ArchiveInstanceInfo](../)
* espace de noms [Aspose.Zip.ArchiveInfo](../../archiveinstanceinfo/)
* Assemblée [Aspose.Zip](../../../)


