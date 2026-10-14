---
title: "IsoArchive.CreateEntry"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode IsoArchive. Ajoute un fichier à l'image ISO"
type: docs
weight: 40
url: /fr/net/aspose.zip.iso/isoarchive/createentry/
---
## CreateEntry(string, string) {#createentry_2}

Ajoute un fichier à l'image ISO.

```csharp
public IsoEntry CreateEntry(string name, string filePath)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Chemin du fichier dans l'ISO. |
| filePath | String | Chemin du fichier. |

### Valeur de retour

L'entrée ISO composée.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | Le *filePath* est nul. |
| ArgumentException | Le *filePath* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *filePath* est refusé. |
| PathTooLongException | Le *filePath* spécifié dépasse la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *filePath* contient deux‑points (:) au milieu de la chaîne. |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, (par exemple, il se trouve sur un lecteur non mappé). |
| FileNotFoundException | Le fichier spécifié dans *filePath* est introuvable. |
| InvalidOperationException | L'archive n'est pas en mode édition. |

### Voir aussi

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string, Stream) {#createentry_1}

Ajoute un fichier à l'image ISO.

```csharp
public IsoEntry CreateEntry(string name, Stream source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Chemin du fichier dans l'ISO. |
| source | Stream | Flux contenant les données du fichier. |

### Valeur de retour

L'entrée ISO composée.

### Exceptions

| exception | condition |
| --- | --- |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |
| ArgumentNullException | Lancé lorsque *name* ou *source* est nul. |
| InvalidOperationException | L'archive n'est pas en mode édition. |

### Voir aussi

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)

---

## CreateEntry(string) {#createentry}

Ajoute un fichier à l'image ISO.

```csharp
public IsoEntry CreateEntry(string name)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| name | String | Chemin du répertoire dans l'ISO. |

### Valeur de retour

L'entrée ISO composée.

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | `name` est nul ou vide. |
| InvalidOperationException | L'archive est ouverte pour l'extraction. |
| ObjectDisposedException | L'archive a été libérée et ne peut pas être utilisée. |

### Voir aussi

* class [IsoEntry](../../isoentry/)
* class [IsoArchive](../)
* namespace [Aspose.Zip.Iso](../../isoarchive/)
* assembly [Aspose.Zip](../../../)


