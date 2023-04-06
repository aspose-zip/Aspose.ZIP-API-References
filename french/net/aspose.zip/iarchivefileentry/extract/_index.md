---
title: IArchiveFileEntry.Extract
second_title: Référence de l'API Aspose.ZIP pour .NET
description: IArchiveFileEntry méthode. Extrait lentrée du système de fichiers par le chemin fourni.
type: docs
weight: 30
url: /fr/net/aspose.zip/iarchivefileentry/extract/
---
## Extract(string) {#extract}

Extrait l'entrée du système de fichiers par le chemin fourni.

```csharp
public FileInfo Extract(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier de destination. Si le fichier existe déjà, il sera écrasé. |

### Return_Value

FileInfo instance contenant les données extraites.

### Voir également

* interface [IArchiveFileEntry](../)
* espace de noms [Aspose.Zip](../../iarchivefileentry/)
* Assemblée [Aspose.Zip](../../../)

---

## Extract(Stream) {#extract_1}

Extrait l'entrée du flux fourni.

```csharp
public void Extract(Stream destination)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| destination | Stream | Flux de destination. Doit être inscriptible. |

### Voir également

* interface [IArchiveFileEntry](../)
* espace de noms [Aspose.Zip](../../iarchivefileentry/)
* Assemblée [Aspose.Zip](../../../)


