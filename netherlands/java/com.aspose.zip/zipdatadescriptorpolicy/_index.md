---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor de aanwezigheid van Data Descriptor."
type: docs
weight: 171
url: /nl/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Opties voor de aanwezigheid van Data Descriptor.
## Velden

| Veld | Beschrijving |
| --- | --- |
| [Always](#Always) | Data Descriptor is altijd aanwezig voor alle zip-items. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor alleen aanwezig voor items met bestandsgegevens; weggelaten voor mappen. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor is altijd aanwezig voor alle zip-items.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor alleen aanwezig voor items met bestandsgegevens; weggelaten voor mappen. Het gebruik van deze optie wordt afgeraden.

Kan alleen worden toegepast op niet-versleutelde archieven.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| naam | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
