---
title: "PPMdCompressionSettings"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Pengaturan untuk kompresi PPMd dalam arsip ZIP."
type: docs
weight: 93
url: /id/java/com.aspose.zip/ppmdcompressionsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.zip.CompressionSettings](../../com.aspose.zip/compressionsettings)
```
public class PPMdCompressionSettings extends CompressionSettings
```

Pengaturan untuk kompresi PPMd dalam arsip ZIP.

PPMd adalah algoritma kompresi data yang dikembangkan oleh Dmitry Shkarin. Algoritma ini didasarkan pada pencocokan frasa prediktif pada beberapa konteks urutan.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PPMdCompressionSettings(int modelOrder, int suballocatorSize)](#PPMdCompressionSettings-int-int-) | Menginisialisasi instance baru dari kelas [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings). |
| [PPMdCompressionSettings()](#PPMdCompressionSettings--) | Menginisialisasi instance baru dari kelas [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings) dengan urutan model default dan ukuran sub-allocator default. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getModelOrder()](#getModelOrder--) | Mendapatkan urutan model. |
| [getSuballocatorSize()](#getSuballocatorSize--) | Mendapatkan ukuran sub-allocator dalam MB. |
### PPMdCompressionSettings(int modelOrder, int suballocatorSize) {#PPMdCompressionSettings-int-int-}
```
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```


Menginisialisasi instance baru dari kelas [PPMdCompressionSettings](../../com.aspose.zip/ppmdcompressionsettings).

```

``````

try (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10)))) {
archive.createEntry("data.bin", "data.bin");
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

Urutan model default adalah 8, dan ukuran sub-allocator adalah 50MB.

### getModelOrder() {#getModelOrder--}
```
public final int getModelOrder()
```


Mendapatkan urutan model.

**Returns:**
int - urutan model
### getSuballocatorSize() {#getSuballocatorSize--}
```
public final int getSuballocatorSize()
```


Mendapatkan ukuran sub-allocator dalam MB.

**Returns:**
int - ukuran sub-allocator dalam MB
