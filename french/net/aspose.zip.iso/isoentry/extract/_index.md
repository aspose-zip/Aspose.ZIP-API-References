---
title: "IsoEntry.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode IsoEntry. Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni"
type: docs
weight: 50
url: /fr/net/aspose.zip.iso/isoentry/extract/
---
## Extract(string) {#extract}

Extrait l'entrée dans le système de fichiers au chemin fourni.

```csharp
public FileInfo Extract(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

### Valeur de retour

Instance FileInfo contenant les données extraites.

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
| InvalidOperationException | Les en-têtes d'archive et les informations de service n'ont pas été lus. |

### Voir aussi

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrait l'entrée vers le flux fourni.

```csharp
public void Extract(Stream destination)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être accessible en écriture. |

### Exceptions

| exception | condition |
| --- | --- |
| NotSupportedException | Lève une exception si l'entrée ne représente pas un fichier. |
| ArgumentException | Le flux fourni ne prend pas en charge l'écriture. |

### Voir aussi

* class [IsoEntry](../)
* namespace [Aspose.Zip.Iso](../../isoentry/)
* assembly [Aspose.Zip](../../../)


