---
title: "TarArchive.FromLZ4"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode TarArchive. Extrait l'archive LZ4 fournie et compose un TarArchive à partir des données extraites"
type: docs
weight: 30
url: /fr/net/aspose.zip.tar/tararchive/fromlz4/
---
## FromLZ4(string) {#fromlz4_1}

Extrait l'archive LZ4 fournie et compose [`TarArchive`](../) à partir des données extraites.

Important : l'archive LZ4 est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromLZ4(string path)
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
| SecurityException | L'appelant n'a pas l'autorisation requise pour accéder |
| ArgumentException | Le *path* est vide, ne contient que des espaces blancs ou contient des caractères invalides. |
| UnauthorizedAccessException | L'accès au fichier *path* est refusé. |
| PathTooLongException | Le *path* spécifié, le nom de fichier, ou les deux dépassent la longueur maximale définie par le système. Par exemple, sur les plates‑formes Windows, les chemins doivent contenir moins de 248 caractères et les noms de fichier moins de 260 caractères. |
| NotSupportedException | Le fichier à *path* est dans un format invalide. |
| DirectoryNotFoundException | Le chemin spécifié est invalide, par exemple s'il se trouve sur un lecteur non mappé. |
| FileNotFoundException | Le fichier est introuvable. |
| EndOfStreamException | Le fichier est trop court. |
| InvalidDataException | Le fichier a une signature incorrecte. |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |
| InvalidOperationException | L'archive est préparée pour la composition. |

## Remarques

Le flux d'extraction LZ4 n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne.

### Voir aussi

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZ4(Stream) {#fromlz4}

Extrait l'archive LZ4 fournie et compose [`TarArchive`](../) à partir des données extraites.

Important : l'archive LZ4 est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromLZ4(Stream source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Stream | La source de l'archive. |

### Valeur de retour

Une instance de [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentException | Impossible de lire depuis *source* |
| ArgumentNullException | *source* est nul. |
| EndOfStreamException | *source* est trop court. |
| InvalidDataException | Le *source* a une signature incorrecte. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |

## Remarques

Le flux d'extraction LZ4 n'est pas positionnable en raison de la nature de l'algorithme de compression. L'archive Tar offre la possibilité d'extraire un enregistrement arbitraire, il doit donc fonctionner avec un flux positionnable en interne.

### Voir aussi

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


