---
title: "TarArchive.FromLZMA"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode TarArchive. Extrait l'archive LZMA fournie et compose un TarArchive à partir des données extraites"
type: docs
weight: 50
url: /fr/net/aspose.zip.tar/tararchive/fromlzma/
---
## FromLZMA(Stream) {#fromlzma}

Extrait l'archive LZMA fournie et compose [`TarArchive`](../) à partir des données extraites.

Important: l'archive LZMA est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromLZMA(Stream source)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| source | Stream | La source de l'archive. |

### Valeur de retour

Une instance de [`TarArchive`](../)

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | L'archive est corrompue. |
| EndOfStreamException | Lancé lorsque la fin du flux est atteinte avant que le nombre attendu d'octets ne soit lu. |
| ObjectDisposedException | Lancée si le flux source a été libéré. |
| ArgumentNullException | *source* est nul. |
| IOException | Une erreur d'E/S se produit. |

## Remarques

Le flux d'extraction LZMA n'est pas recherchable en raison de la nature de l'algorithme de compression. L'archive Tar fournit une fonctionnalité d'extraction d'enregistrement arbitraire, il doit donc fonctionner avec un flux recherchable en interne.

### Voir aussi

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)

---

## FromLZMA(string) {#fromlzma_1}

Extrait l'archive LZMA fournie et compose [`TarArchive`](../) à partir des données extraites.

Important: l'archive LZMA est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromLZMA(string path)
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
| EndOfStreamException | Lancé lorsque la fin du flux est atteinte avant que le nombre attendu d'octets ne soit lu. |
| IOException | Une erreur d'E/S s'est produite lors de l'ouverture du fichier. |
| InvalidDataException | L'archive est corrompue. |

## Remarques

Le flux d'extraction LZMA n'est pas recherchable en raison de la nature de l'algorithme de compression. L'archive Tar fournit une fonctionnalité d'extraction d'enregistrement arbitraire, il doit donc fonctionner avec un flux recherchable en interne.

### Voir aussi

* class [TarArchive](../)
* namespace [Aspose.Zip.Tar](../../tararchive/)
* assembly [Aspose.Zip](../../../)


