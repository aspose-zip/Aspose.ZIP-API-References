---
title: "UueSaveOptions"
second_title: "Riferimento API di Aspose.ZIP for Java"
description: "Opzioni per salvare un file uuencoded."
type: docs
weight: 129
url: /it/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Opzioni per salvare un file uuencoded.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Inizializza le opzioni con il nome file fornito dall'utente e una nuova riga. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Inizializza le opzioni con il nome file fornito dall'utente e la nuova riga predefinita. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [getFileName()](#getFileName--) | Ottiene il nome file da utilizzare durante la ricreazione dei dati decodificati. |
| [getNewLine()](#getNewLine--) | Ottiene il carattere che termina ogni riga, solitamente "\n" o "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Ottiene i permessi Unix del file. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Imposta i permessi Unix del file. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Inizializza le opzioni con il nome file fornito dall'utente e una nuova riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | il nome file da utilizzare durante la ricreazione dei dati decodificati |
| newLine | java.lang.String | il carattere che termina ogni riga |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Inizializza le opzioni con il nome file fornito dall'utente e la nuova riga predefinita.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fileName | java.lang.String | il nome file da utilizzare durante la ricreazione dei dati decodificati |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Ottiene il nome file da utilizzare durante la ricreazione dei dati decodificati.

**Returns:**
java.lang.String - il nome file da utilizzare durante la ricreazione dei dati decodificati
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Ottiene il carattere che termina ogni riga, solitamente "\n" o "\r\n".

**Returns:**
java.lang.String - il carattere che termina ogni riga, solitamente "\n" o "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Ottiene i permessi Unix del file.

Il valore predefinito è 644.

**Returns:**
java.lang.String - i permessi Unix del file
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Imposta i permessi Unix del file.

Il valore predefinito è 644.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String | i permessi Unix del file |

