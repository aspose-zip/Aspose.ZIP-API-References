---
title: TarArchive.FromGZip
second_title: Référence de l'API Aspose.ZIP pour .NET
description: TarArchive méthode. Extrait larchive gzip fournie et composeTarArchive à partir des données extraites.
type: docs
weight: 20
url: /fr/net/aspose.zip.tar/tararchive/fromgzip/
---
## FromGZip(Stream) {#fromgzip}

Extrait l'archive gzip fournie et compose[`TarArchive`](../) à partir des données extraites.

Important : l'archive gzip est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromGZip(Stream source)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| source | Stream | La source des archives. |

### Return_Value

Un exemple de[`TarArchive`](../)

### Remarques

Le flux d'extraction GZip n'est pas recherchable par la nature de l'algorithme de compression. L'archive Tar fournit la possibilité d'extraire un enregistrement arbitraire, elle doit donc exploiter un flux recherchable sous le capot.

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)

---

## FromGZip(string) {#fromgzip_1}

Extrait l'archive gzip fournie et compose[`TarArchive`](../) à partir des données extraites.

Important : l'archive gzip est entièrement extraite dans cette méthode, son contenu est conservé en interne. Attention à la consommation de mémoire.

```csharp
public static TarArchive FromGZip(string path)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| path | String | Chemin d'accès au fichier d'archive. |

### Return_Value

Un exemple de[`TarArchive`](../)

### Remarques

Le flux d'extraction GZip n'est pas recherchable par la nature de l'algorithme de compression. L'archive Tar fournit la possibilité d'extraire un enregistrement arbitraire, elle doit donc exploiter un flux recherchable sous le capot.

### Voir également

* class [TarArchive](../)
* espace de noms [Aspose.Zip.Tar](../../tararchive/)
* Assemblée [Aspose.Zip](../../../)


