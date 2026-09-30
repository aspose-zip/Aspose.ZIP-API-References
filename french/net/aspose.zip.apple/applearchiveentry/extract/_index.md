---
title: "AppleArchiveEntry.Extract"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode AppleArchiveEntry. Extrait l'entrée vers le système de fichiers en utilisant le chemin fourni"
type: docs
weight: 50
url: /fr/net/aspose.zip.apple/applearchiveentry/extract/
---
## Extract(string) {#extract}

Extrait l'entrée dans le système de fichiers au chemin fourni.

```csharp
public FileInfo Extract(string path)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| chemin | String | Le chemin du fichier de destination. Si le fichier existe déjà, il sera écrasé. |

### Exceptions

| exception | condition |
| --- | --- |
| InvalidDataException | La somme de contrôle ou le condensat stocké pour l'entrée ne correspond pas aux données extraites. |
| InvalidOperationException | L'entrée appartient à une archive préparée pour la composition, ou les données de l'entrée ne peuvent pas être ouvertes à partir d'un flux d'archive non recherchable. |
| NotSupportedException | L'entrée appartient à une archive Apple solide ou utilise une méthode de compression non prise en charge. |
| ObjectDisposedException | Le flux source a été libéré. |
| IOException | Une erreur d'E/S se produit. |

### Voir aussi

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
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
| ArgumentNullException | *destination* est `null`. |
| ArgumentException | *destination* ne prend pas en charge l'écriture. |
| InvalidDataException | La somme de contrôle ou le condensat stocké pour l'entrée ne correspond pas aux données extraites. |
| InvalidOperationException | L'entrée appartient à une archive préparée pour la composition, ou les données de l'entrée ne peuvent pas être ouvertes à partir d'un flux d'archive non recherchable. |
| NotSupportedException | L'entrée appartient à une archive Apple solide ou utilise une méthode de compression non prise en charge. |
| ObjectDisposedException | Le flux source a été libéré. |
| IOException | Une erreur d'E/S se produit. |

### Voir aussi

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


