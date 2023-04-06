---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Référence de l'API Aspose.ZIP pour .NET
description: SevenZipPPMdCompressionSettings constructeur. Instancie les paramètres de la méthode de compression PPMd dans larchive 7z.
type: docs
weight: 10
url: /fr/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

Instancie les paramètres de la méthode de compression PPMd dans l'archive 7z.

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| Paramètre | Taper | La description |
| --- | --- | --- |
| maxOrder | Byte | Commande maximale. |
| suballocatorSize | Int32 | La taille de la mémoire en Mo peut être consommée par le sous-allocateur. |

### Exceptions

| exception | condition |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* n'est pas compris entre 2 et 32, ou*suballocatorSize* n'est pas compris entre 1 et 1024. |

### Remarques

Des commandes de modèles plus importantes entraînent presque sûrement une meilleure compression et sûrement plus d'utilisation de la mémoire et du processeur.

L'algorithme PPMd peut avoir besoin de beaucoup de mémoire, en particulier lorsqu'il est utilisé sur des fichiers volumineux et/ou avec une grande commande de modèles. Si ppmd a besoin de plus de mémoire que vous ne lui en donnez, la compression sera pire.

### Exemples

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Voir également

* class [SevenZipPPMdCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* Assemblée [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

Instancie les paramètres de la méthode de compression PPMd dans l'archive 7z avec l'ordre du modèle par défaut et la taille du sous-allocateur.

```csharp
public SevenZipPPMdCompressionSettings()
```

### Remarques

L'ordre du modèle par défaut est 6 et la taille du sous-allocateur est de 16 Mo.

### Exemples

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### Voir également

* class [SevenZipPPMdCompressionSettings](../)
* espace de noms [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* Assemblée [Aspose.Zip](../../../)


