---
title: "ZipDataDescriptorPolicy"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen für das Vorhandensein des Data Descriptors."
type: docs
weight: 171
url: /de/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Optionen für das Vorhandensein des Data Descriptors.
## Felder

| Feld | Beschreibung |
| --- | --- |
| [Always](#Always) | Data Descriptor ist immer für alle Zip-Einträge vorhanden. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor ist nur für Einträge mit Dateidaten vorhanden; für Verzeichnisse weggelassen. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor ist immer für alle Zip-Einträge vorhanden.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor ist nur für Einträge mit Dateidaten vorhanden; für Verzeichnisse weggelassen. Die Verwendung dieser Option wird nicht empfohlen.

Kann nur auf nicht verschlüsselte Archive angewendet werden.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Name | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
