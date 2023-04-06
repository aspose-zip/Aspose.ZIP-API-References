---
title: MeteredLicense.SetMeteredKey
second_title: Référence de l'API Aspose.ZIP pour .NET
description: MeteredLicense méthode. Définit une clé publique et privée mesurée.
type: docs
weight: 20
url: /fr/net/aspose.zip/meteredlicense/setmeteredkey/
---
## MeteredLicense.SetMeteredKey method

Définit une clé publique et privée mesurée.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| publicKey | String | La clé publique. |
| privateKey | String | La clé privée. |

### Remarques

Si vous achetez une licence limitée, lorsque vous démarrez l'application, cette API doit être appelée, normalement, cela suffit. Cependant, si vous ne parvenez toujours pas à télécharger les données de consommation et dépassez 24 heures, la licence sera définie sur le statut d'évaluation, pour éviter un tel cas, vous devez vérifier régulièrement le statut de la licence, s'il s'agit du statut d'évaluation, appelez à nouveau cette API.

### Voir également

* class [MeteredLicense](../)
* espace de noms [Aspose.Zip](../../meteredlicense/)
* Assemblée [Aspose.Zip](../../../)


