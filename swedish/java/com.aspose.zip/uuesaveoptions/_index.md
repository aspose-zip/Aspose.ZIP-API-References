---
title: "UueSaveOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ för att spara en uu-kodad fil."
type: docs
weight: 129
url: /sv/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Alternativ för att spara en uu-kodad fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Initierar alternativen med användarens angivna filnamn och ny rad. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Initierar alternativen med användarens angivna filnamn och standardny rad. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getFileName()](#getFileName--) | Hämtar filnamnet som ska användas när den avkodade datan återskapas. |
| [getNewLine()](#getNewLine--) | Hämtar tecknet som avslutar varje rad, vanligtvis "\n" eller "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Hämtar filens Unix-filbehörigheter. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Ställer in filens Unix-filbehörigheter. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Initierar alternativen med användarens angivna filnamn och ny rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | filnamnet som ska användas när den avkodade datan återskapas |
| newLine | java.lang.String | tecknet som avslutar varje rad |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Initierar alternativen med användarens angivna filnamn och standardny rad.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fileName | java.lang.String | filnamnet som ska användas när den avkodade datan återskapas |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Hämtar filnamnet som ska användas när den avkodade datan återskapas.

**Returns:**
java.lang.String - filnamnet som ska användas när den avkodade datan återskapas
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Hämtar tecknet som avslutar varje rad, vanligtvis "\n" eller "\r\n".

**Returns:**
java.lang.String - tecknet som avslutar varje rad, vanligtvis "\n" eller "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Hämtar filens Unix-filbehörigheter.

Standard är 644.

**Returns:**
java.lang.String - filens Unix-filbehörigheter
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Ställer in filens Unix-filbehörigheter.

Standard är 644.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | filens Unix-filbehörigheter |

