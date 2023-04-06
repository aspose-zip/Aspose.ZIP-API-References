---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: PPMdCompressionSettings constructeur. Initialise une nouvelle instance duPPMdCompressionSettings classe.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

Initialise une nouvelle instance du[`PPMdCompressionSettings`](../) classe.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| modelOrder | Int32 | Commande du modèle. |
| suballocatorSize | Int32 | La taille de la mémoire en Mo peut être consommée par le sous-allocateur. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* n'est pas compris entre 2 et 16. - ou -*suballocatorSize* n'est pas compris entre 1 et 256. |

### Remarques

Des commandes de modèles plus importantes entraînent presque sûrement une meilleure compression et sûrement plus d'utilisation de la mémoire et du processeur.

L'algorithme PPMd peut avoir besoin de beaucoup de mémoire, en particulier lorsqu'il est utilisé sur des fichiers volumineux et/ou avec une grande commande de modèles. Si ppmd a besoin de plus de mémoire que vous ne lui en donnez, la compression sera pire.

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Voir également

* class [PPMdCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* Assemblée [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

Initialise une nouvelle instance du[`PPMdCompressionSettings`](../) classe avec l'ordre du modèle par défaut et la taille du sous-allocateur.

```csharp
public PPMdCompressionSettings()
```

### Remarques

L'ordre du modèle par défaut est 8 et la taille du sous-allocateur est de 50 Mo.

### Exemples

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### Voir également

* class [PPMdCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* Assemblée [Aspose.Zip](../../../)


