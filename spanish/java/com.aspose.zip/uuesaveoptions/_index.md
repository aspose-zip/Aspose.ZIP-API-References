---
title: "UueSaveOptions"
second_title: "Referencia de API de Aspose.ZIP para Java"
description: "Opciones para guardar un archivo uuencoded."
type: docs
weight: 129
url: /es/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Opciones para guardar un archivo uuencoded.
## Constructores

| Constructor | Descripción |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Inicializa las opciones con el nombre de archivo proporcionado por el usuario y una nueva línea. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Inicializa las opciones con el nombre de archivo proporcionado por el usuario y la nueva línea predeterminada. |
## Métodos

| Método | Descripción |
| --- | --- |
| [getFileName()](#getFileName--) | Obtiene el nombre de archivo que se usará al recrear los datos decodificados. |
| [getNewLine()](#getNewLine--) | Obtiene el carácter que termina cada línea, usualmente "\n" o "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Obtiene los permisos de archivo Unix del archivo. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Establece los permisos Unix del archivo. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Inicializa las opciones con el nombre de archivo proporcionado por el usuario y una nueva línea.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | el nombre del archivo que se usará al recrear los datos decodificados |
| newLine | java.lang.String | el carácter que termina cada línea |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Inicializa las opciones con el nombre de archivo proporcionado por el usuario y la nueva línea predeterminada.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fileName | java.lang.String | el nombre del archivo que se usará al recrear los datos decodificados |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Obtiene el nombre de archivo que se usará al recrear los datos decodificados.

**Returns:**
java.lang.String - el nombre del archivo que se usará al recrear los datos decodificados
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Obtiene el carácter que termina cada línea, usualmente "\n" o "\r\n".

**Returns:**
java.lang.String - el carácter que termina cada línea, usualmente "\n" o "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Obtiene los permisos de archivo Unix del archivo.

El valor predeterminado es 644.

**Returns:**
java.lang.String - los permisos Unix del archivo
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Establece los permisos Unix del archivo.

El valor predeterminado es 644.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String | los permisos Unix del archivo |

