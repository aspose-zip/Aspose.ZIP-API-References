---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API-Referenz"
description: "Optionen, mit denen ein ALZ-Archiv aus einer komprimierten Datei geladen wird."
type: docs
weight: 12
url: /de/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Optionen, mit denen ein ALZ-Archiv aus einer komprimierten Datei geladen wird.
## Konstruktoren

| Konstruktor | Beschreibung |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Liefert das Passwort, das zum Entschlüsseln von Einträgen verwendet wird. |
| [getEncoding()](#getEncoding--) | Liefert die für Eintragsnamen verwendete Kodierung. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Liefert, ob die Prüfsummenüberprüfung von ALZ-Einträgen übersprungen wird. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Setzt ein Abbruch-Flag, das zum Abbrechen der Extraktion verwendet wird. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Setzt das Passwort, das zum Entschlüsseln von Einträgen verwendet wird. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Setzt die für Eintragsnamen verwendete Kodierung. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Setzt, ob die Prüfsummenüberprüfung von ALZ-Einträgen übersprungen wird. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Liefert das Passwort, das zum Entschlüsseln von Einträgen verwendet wird.

**Returns:**
java.lang.String – Passwort, das zum Entschlüsseln von Einträgen verwendet wird, oder `null`, wenn keines konfiguriert ist
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Liefert die für Eintragsnamen verwendete Kodierung. Standard ist die koreanische Windows-Codepage 949 (CP949). ALZ-Archive speichern Dateinamen historisch mit der koreanischen Windows-ANSI-Codepage.

**Returns:**
java.nio.charset.Charset – für Eintragsnamen verwendete Kodierung
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Liefert, ob die Prüfsummenüberprüfung von ALZ-Einträgen übersprungen wird. Standard ist `false`.

**Returns:**
boolean – ob die Prüfsummenüberprüfung übersprungen wird
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Setzt ein Abbruch-Flag, das zum Abbrechen der Extraktion verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | Abbruch-Flag, oder `null`, um den Abbruch zu deaktivieren |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Setzt das Passwort, das zum Entschlüsseln von Einträgen verwendet wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String | Passwort, das zum Entschlüsseln von Einträgen verwendet wird |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Setzt die für Eintragsnamen verwendete Kodierung. ALZ-Archive speichern Dateinamen historisch mit der koreanischen Windows-ANSI-Codepage.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.nio.charset.Charset | Kodierung, die für Eintragsnamen verwendet wird |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Setzt, ob die Prüfsummenüberprüfung von ALZ-Einträgen übersprungen wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean | ob die Prüfsummenüberprüfung übersprungen wird |

