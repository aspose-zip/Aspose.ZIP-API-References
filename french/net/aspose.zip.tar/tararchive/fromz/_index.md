---
title: TarArchive.FromZ
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Extrait larchive au format Z fournie et composeTarArchive à partir des données extraites.
type: docs
weight: 50
url: /fr/net/aspose.zip.tar/tararchive/fromz/
---
## FromZ(Stream) {#fromz}

Extrait l'archive au format Z fournie et compose[`TarArchive`](../) à partir des données extraites.

Important : L'archive Z est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromZ(Stream source)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| source | Stream | La source des archives. |

### Return_Value

Un exemple de[`TarArchive`](../)

### Remarques

L'archive Tar fournit la possibilité d'extraire un enregistrement arbitraire, elle doit donc exploiter un flux consultable sous le capot.

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## FromZ(string) {#fromz_1}

Extrait l'archive au format Z fournie et compose[`TarArchive`](../) à partir des données extraites.

Important : L'archive Z est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromZ(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier d'archive. |

### Return_Value

Un exemple de[`TarArchive`](../)

### Remarques

L'archive Tar fournit la possibilité d'extraire un enregistrement arbitraire, elle doit donc exploiter un flux consultable sous le capot.

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


