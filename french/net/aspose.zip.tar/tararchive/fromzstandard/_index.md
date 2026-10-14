---
title: "TarArchive.FromZstandard"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode TarArchive. Extrait l'archive Zstandard fournie et compose un TarArchive à partir des données extraites."
type: docs
weight: 80
url: /fr/net/aspose.zip.tar/tararchive/fromzstandard/
---
## FromZstandard(Stream) {#fromzstandard}

Extrait l'archive Zstandard fournie et compose [`TarArchive`](../) à partir des données extraites.

Important: l'archive Zstandard est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromZstandard(Stream source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Stream | La source de l'archive. |

### Valeur de retour

Une instance de [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| IOException | Le flux Zstandard est corrompu ou illisible. |
| InvalidDataException | Les données sont corrompues. |
| EndOfStreamException | Lancé lorsque la fin du flux est atteinte avant que le nombre attendu d'octets ne soit lu. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |

### Voir aussi

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromZstandard(string) {#fromzstandard_1}

Extrait l'archive Zstandard fournie et compose [`TarArchive`](../) à partir des données extraites.

Important: l'archive Zstandard est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromZstandard(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin vers le fichier d'archive. |

### Valeur de retour

Une instance de [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentNullException | *path* est nul. |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* est dans un format invalide. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| FileNotFoundException | Le fichier est introuvable. |
| IOException | Le flux Zstandard est corrompu ou illisible. |
| InvalidDataException | Les données sont corrompues. |
| EndOfStreamException | Lancé lorsque la fin du flux est atteinte avant que le nombre attendu d'octets ne soit lu. |

### Voir aussi

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


