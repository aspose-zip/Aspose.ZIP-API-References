---
title: "ZipDataDescriptorPolicy"
second_title: "Referensi API Aspose.ZIP untuk Java"
description: "Opsi untuk keberadaan Data Descriptor."
type: docs
weight: 171
url: /id/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Opsi untuk keberadaan Data Descriptor.
## Fields

| Field | Deskripsi |
| --- | --- |
| [Always](#Always) | Data Descriptor selalu hadir untuk semua entri zip. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor hadir hanya untuk entri dengan data file; diabaikan untuk direktori. |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor selalu hadir untuk semua entri zip.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor hadir hanya untuk entri dengan data file; diabaikan untuk direktori. Penggunaan opsi ini tidak disarankan.

Hanya dapat diterapkan pada arsip yang tidak terenkripsi.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nama | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
