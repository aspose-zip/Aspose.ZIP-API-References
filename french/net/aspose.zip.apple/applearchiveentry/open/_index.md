---
title: "AppleArchiveEntry.Open"
second_title: "Référence de l'API Aspose.ZIP pour .NET"
description: "Méthode AppleArchiveEntry. Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée"
type: docs
weight: 60
url: /fr/net/aspose.zip.apple/applearchiveentry/open/
---
## AppleArchiveEntry.Open method

Ouvre l'entrée pour l'extraction et fournit un flux contenant le contenu de l'entrée.

```csharp
public Stream Open()
```

### Valeur de retour

Un flux lisible qui contient les données extraites de l'entrée.

### Exceptions

| exception | condition |
| --- | --- |
| NotSupportedException | L'entrée appartient à une archive Apple solide ou utilise une méthode de compression non prise en charge. |
| InvalidDataException | La somme de contrôle ou le condensat stocké pour l'entrée ne correspond pas aux données extraites. |
| InvalidOperationException | L'entrée appartient à une archive préparée pour la composition, ou les données de l'entrée ne peuvent pas être ouvertes à partir d'un flux d'archive non recherchable. |
| ObjectDisposedException | Le flux source a été libéré. |
| IOException | Une erreur d'E/S se produit. |

## Remarques

Lisez le flux retourné pour obtenir le contenu original de l'entrée. Si l'archive contient des champs de somme de contrôle, la somme de contrôle est vérifiée pendant la lecture du flux retourné.

### Voir aussi

* class [AppleArchiveEntry](../)
* namespace [Aspose.Zip.Apple](../../applearchiveentry/)
* assembly [Aspose.Zip](../../../)


