---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för närvaro av Data Descriptor."
type: docs
weight: 171
url: /sv/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Alternativ för närvaro av Data Descriptor.
## Fält

| Fält | Beskrivning |
| --- | --- |
| [Always](#Always) | Data Descriptor är alltid närvarande för alla zip-poster. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor finns endast för poster med fildata; utelämnas för kataloger. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor är alltid närvarande för alla zip-poster.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor finns endast för poster med fildata; utelämnas för kataloger. Användning av detta alternativ avråds.

Kan endast tillämpas på icke-krypterade arkiv.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| namn | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
