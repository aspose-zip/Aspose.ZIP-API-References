---
title: "UueSaveOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen zum Speichern einer uuencodierten Datei."
type: docs
weight: 129
url: /de/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Optionen zum Speichern einer uuencodierten Datei.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Initialisiert die Optionen mit dem vom Benutzer angegebenen Dateinamen und einem Zeilenumbruch. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Initialisiert die Optionen mit dem vom Benutzer angegebenen Dateinamen und dem Standard-Zeilenumbruch. |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getFileName()](#getFileName--) | Liefert den Dateinamen, der beim Wiederherstellen der dekodierten Daten verwendet wird. |
| [getNewLine()](#getNewLine--) | Liefert das Zeichen, das jede Zeile beendet, normalerweise "\n" oder "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Liefert die Unix-Dateiberechtigungen der Datei. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Legt die Unix-Dateiberechtigungen der Datei fest. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Initialisiert die Optionen mit dem vom Benutzer angegebenen Dateinamen und einem Zeilenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname, der beim Wiederherstellen der dekodierten Daten verwendet wird |
| newLine | java.lang.String | Das Zeichen, das jede Zeile beendet |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Initialisiert die Optionen mit dem vom Benutzer angegebenen Dateinamen und dem Standard-Zeilenumbruch.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| fileName | java.lang.String | Der Dateiname, der beim Wiederherstellen der dekodierten Daten verwendet wird |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Liefert den Dateinamen, der beim Wiederherstellen der dekodierten Daten verwendet wird.

**Returns:**
java.lang.String - der Dateiname, der beim Wiederherstellen der dekodierten Daten verwendet wird
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Liefert das Zeichen, das jede Zeile beendet, normalerweise "\n" oder "\r\n".

**Returns:**
java.lang.String - das Zeichen, das jede Zeile beendet, normalerweise "\n" oder "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Liefert die Unix-Dateiberechtigungen der Datei.

Standard ist 644.

**Returns:**
java.lang.String - die Unix-Dateiberechtigungen der Datei
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Legt die Unix-Dateiberechtigungen der Datei fest.

Standard ist 644.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | die Unix-Dateiberechtigungen der Datei |

