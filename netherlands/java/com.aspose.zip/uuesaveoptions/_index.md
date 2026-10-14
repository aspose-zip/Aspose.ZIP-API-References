---
title: "UueSaveOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties voor het opslaan van een uuencoded-bestand."
type: docs
weight: 129
url: /nl/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Opties voor het opslaan van een uuencoded-bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Initialiseert de opties met een door de gebruiker opgegeven bestandsnaam en een nieuwe regel. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Initialiseert de opties met een door de gebruiker opgegeven bestandsnaam en de standaard nieuwe regel. |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getFileName()](#getFileName--) | Haalt de bestandsnaam op die gebruikt wordt bij het opnieuw creëren van de gedecodeerde gegevens. |
| [getNewLine()](#getNewLine--) | Haalt het teken op dat elke regel beëindigt, meestal "\n" of "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Haalt de Unix-bestandsmachtigingen van het bestand op. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Stelt de Unix-bestandsmachtigingen van het bestand in. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Initialiseert de opties met een door de gebruiker opgegeven bestandsnaam en een nieuwe regel.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | de bestandsnaam die moet worden gebruikt bij het opnieuw maken van de gedecodeerde gegevens |
| newLine | java.lang.String | het teken dat elke regel beëindigt |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Initialiseert de opties met een door de gebruiker opgegeven bestandsnaam en de standaard nieuwe regel.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| fileName | java.lang.String | de bestandsnaam die moet worden gebruikt bij het opnieuw maken van de gedecodeerde gegevens |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Haalt de bestandsnaam op die gebruikt wordt bij het opnieuw creëren van de gedecodeerde gegevens.

**Returns:**
java.lang.String - de bestandsnaam die moet worden gebruikt bij het opnieuw maken van de gedecodeerde gegevens
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Haalt het teken op dat elke regel beëindigt, meestal "\n" of "\r\n".

**Returns:**
java.lang.String - het teken dat elke regel beëindigt, meestal "\n" of "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Haalt de Unix-bestandsmachtigingen van het bestand op.

Standaard is 644.

**Returns:**
java.lang.String - de Unix-bestandsmachtigingen van het bestand
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Stelt de Unix-bestandsmachtigingen van het bestand in.

Standaard is 644.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | de Unix-bestandsmachtigingen van het bestand |

