---
title: ZipDataDescriptorPolicy
second_title: Aspose.ZIP for Java API Reference
description: Options for the Data Descriptor presence.
type: docs
weight: 147
url: /java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Options for the Data Descriptor presence.
## Fields

| Field | Description |
| --- | --- |
| [Always](#Always) | Data Descriptor is always present for all zip entries. |
| [ForAllFileEntries](#ForAllFileEntries) | Data Descriptor present only for entries with file data; omitted for directories. |
## Methods

| Method | Description |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


Data Descriptor is always present for all zip entries.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Data Descriptor present only for entries with file data; omitted for directories. Usage of this option is discouraged.

Can only be applied to non-encrypted archives.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
