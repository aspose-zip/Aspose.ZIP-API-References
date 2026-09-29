---
title: "ZipDataDescriptorPolicy"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para la presencia del Descriptor de Datos."
type: docs
weight: 171
url: /es/java/com.aspose.zip/zipdatadescriptorpolicy/
---

**Inheritance:**
java.lang.Object, java.lang.Enum
```
public enum ZipDataDescriptorPolicy extends Enum<ZipDataDescriptorPolicy>
```

Opciones para la presencia del Descriptor de Datos.
## Campos

| Campo | Descripción |
| --- | --- |
| [Always](#Always) | El Descriptor de datos siempre está presente para todas las entradas zip. |
| [ForAllFileEntries](#ForAllFileEntries) | Descriptor de datos presente solo para entradas con datos de archivo; omitido para directorios. |
## Métodos

| Método | Descripción |
| --- | --- |
| [valueOf(String name)](#valueOf-java.lang.String-) |  |
| [values()](#values--) |  |
### Always {#Always}
```
public static final ZipDataDescriptorPolicy Always
```


El Descriptor de datos siempre está presente para todas las entradas zip.

### ForAllFileEntries {#ForAllFileEntries}
```
public static final ZipDataDescriptorPolicy ForAllFileEntries
```


Descriptor de datos presente solo para entradas con datos de archivo; omitido para directorios. Se desaconseja el uso de esta opción.

Solo se puede aplicar a archivos no cifrados.

### valueOf(String name) {#valueOf-java.lang.String-}
```
public static ZipDataDescriptorPolicy valueOf(String name)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| nombre | java.lang.String |  |

**Returns:**
[ZipDataDescriptorPolicy](../../com.aspose.zip/zipdatadescriptorpolicy)
### values() {#values--}
```
public static ZipDataDescriptorPolicy[] values()
```




**Returns:**
com.aspose.zip.ZipDataDescriptorPolicy[]
