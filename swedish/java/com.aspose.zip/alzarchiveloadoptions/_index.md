---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP för Java API-referens"
description: "Alternativ med vilka ett ALZ-arkiv laddas från en komprimerad fil."
type: docs
weight: 12
url: /sv/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Alternativ med vilka ett ALZ-arkiv laddas från en komprimerad fil.
## Konstruktörer

| Konstruktor | Beskrivning |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Hämtar lösenordet som används för att dekryptera poster. |
| [getEncoding()](#getEncoding--) | Hämtar kodningen som används för postnamn. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Hämtar om kontrollsummeverifiering av ALZ-poster hoppas över. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Ställer in en avbrytningsflagga som används för att avbryta extraktion. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Ställer in lösenordet som används för att dekryptera poster. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Ställer in kodningen som används för postnamn. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Ställer in om kontrollsummeverifiering av ALZ-poster hoppas över. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Hämtar lösenordet som används för att dekryptera poster.

**Returns:**
java.lang.String - lösenordet som används för att dekryptera poster, eller `null` när inget är konfigurerat
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Hämtar kodningen som används för postnamn. Standard är Koreansk Windows-kodpage 949 (CP949). ALZ-arkiv lagrar historiskt filnamn med den koreanska Windows ANSI-kodpagen.

**Returns:**
java.nio.charset.Charset - kodning som används för postnamn
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Hämtar om kontrollsummeverifiering av ALZ-poster hoppas över. Standard är `false`.

**Returns:**
boolean - om kontrollsummeverifiering hoppas över
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Ställer in en avbrytningsflagga som används för att avbryta extraktion.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | avbrytningsflagga, eller `null` för att inaktivera avbrytning |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Ställer in lösenordet som används för att dekryptera poster.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | lösenord som används för att dekryptera poster |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Ställer in kodningen som används för postnamn. ALZ-arkiv lagrar historiskt filnamn med den koreanska Windows ANSI-kodpagen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.nio.charset.Charset | kodning som används för postnamn |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Ställer in om kontrollsummeverifiering av ALZ-poster hoppas över.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | om kontrollsummeverifiering hoppas över |

