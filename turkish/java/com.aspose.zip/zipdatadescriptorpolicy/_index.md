---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Veri Tanımlayıcısının varlığı için seçenekler."
type: docs
weight: 171
url: /tr/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Veri Tanımlayıcısının varlığı için seçenekler.
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [Always](#Always) | Veri Tanımlayıcı, tüm zip girişleri için her zaman mevcuttur. |
| [ForAllFileEntries](#ForAllFileEntries) | Veri Tanımlayıcı yalnızca dosya verisine sahip girişler için bulunur; dizinler için atlanır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Veri Tanımlayıcı, tüm zip girişleri için her zaman mevcuttur.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Veri Tanımlayıcı yalnızca dosya verisine sahip girişler için bulunur; dizinler için atlanır. Bu seçeneğin kullanımı önerilmez.

Yalnızca şifrelenmemiş arşivlere uygulanabilir.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
