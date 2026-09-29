---
title: "SevenZipPPMdCompressionSettings"
second_title: "Référence API d'Aspose.ZIP for Java"
description: "Paramètres pour la méthode de compression PPMd dans une archive 7z."
type: docs
weight: 117
url: /fr/java/com.aspose.zip/sevenzipppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.SevenZipCompressionSettings](../../com.aspose.zip/sevenzipcompressionsettings)
```
public final class SevenZipPPMdCompressionSettings extends SevenZipCompressionSettings
```

Paramètres pour la méthode de compression PPMd dans une archive 7z.
## Constructeurs

| Constructeur | Description |
| --- | --- |
| [SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)](#SevenZipPPMdCompressionSettings-int-int-) | Instancie les paramètres pour la méthode de compression PPMd dans une archive 7z. |
| [SevenZipPPMdCompressionSettings()](#SevenZipPPMdCompressionSettings--) | Instancie les paramètres pour la méthode de compression PPMd dans une archive 7z avec l'ordre de modèle par défaut et la taille du sous-allocateur. |
## Méthodes

| Méthode | Description |
| --- | --- |
| [getMaxOrder()](#getMaxOrder--) | Obtient l'ordre maximal. |
| [getMethod()](#getMethod--) | Obtient la méthode de compression ou de décompression. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Obtient la taille du sous-allocateur en Mo. |
### SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize) {#SevenZipPPMdCompressionSettings-int-int-}
```
public SevenZipPPMdCompressionSettings(int maxOrder, int suballocatorSize)
```


Instancie les paramètres pour la méthode de compression PPMd dans une archive 7z.

```

``````

try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32)))) {
archive.createEntry(\"data.bin\", \"data.bin\");
archive.save("zipFile.zip");
}
 
```



**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| maxOrder | int | Maximum order.

Bigger model orders almost surely results in better compression and surely more memory and CPU usage. |
| suballocatorSize | int | Memory size in MB suballocator may consume.

The PPMd algorithm might need a lot of memory, especially when used on large files and/or used with large model order. If ppmd needs more memory than you give it, the compression will be worse. |

### SevenZipPPMdCompressionSettings() {#SevenZipPPMdCompressionSettings--}
```
public SevenZipPPMdCompressionSettings()
```


Instantiates settings for PPMd compression method within 7z archive with default model order and sub-allocator size.

```

``````

     try (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings()))) {
         archive.createEntry("data.bin", "data.bin");
         archive.save("sevenZipFile.7z");
     }
 
```

L'ordre de modèle par défaut est 6 et la taille du sous-allocateur est de 16 Mo.

### getMaxOrder() {#getMaxOrder--}
```
public final byte getMaxOrder()
```


Obtient l'ordre maximal.

**Returns:**
byte - l'ordre maximal
### getMethod() {#getMethod--}
```
public SevenZipCompressionMethod getMethod()
```


Obtient la méthode de compression ou de décompression.

**Returns:**
[SevenZipCompressionMethod](../../com.aspose.zip/sevenzipcompressionmethod) - compression or decompression method
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Obtient la taille du sous-allocateur en Mo.

**Returns:**
int - la taille du sous-allocateur en Mo
