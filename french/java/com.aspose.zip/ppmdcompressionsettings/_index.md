---
title: "PPMdCompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la compression PPMd dans une archive ZIP."
type: docs
weight: 93
url: /fr/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Paramètres pour la compression PPMd dans une archive ZIP.

PPMd est un algorithme de compression de données développé par Dmitry Shkarin. Cet algorithme est basé sur la correspondance de phrases prédictives sur des contextes d'ordre multiples.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Initialise une nouvelle instance de la classe [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Initialise une nouvelle instance de la classe [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) avec l'ordre du modèle par défaut et la taille du sous-allocateur. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Obtient l'ordre du modèle. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Obtient la taille du sous-allocateur en Mo. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Initialise une nouvelle instance de la classe [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| modelOrder | int | Order of the model.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### PPMdCompressionSettings() {#PPMdCompressionSettings--}
```
public PPMdCompressionSettings()
```


Initializes a new instance of the [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) class with default model order and sub-allocator size.

```

``````

     try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("zipFile.zip");
     }
 
```

L'ordre du modèle par défaut est 8, et la taille du sous-allocateur est de 50 Mo.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Obtient l'ordre du modèle.

**Returns:**
int - l'ordre du modèle
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Obtient la taille du sous-allocateur en Mo.

**Returns:**
int - la taille du sous-allocateur en Mo
