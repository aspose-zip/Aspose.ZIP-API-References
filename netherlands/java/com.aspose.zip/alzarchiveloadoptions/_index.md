---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Opties waarmee een ALZ-archief wordt geladen vanuit een gecomprimeerd bestand."
type: docs
weight: 12
url: /nl/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Opties waarmee een ALZ-archief wordt geladen vanuit een gecomprimeerd bestand.
## Constructors

| Constructor | Beschrijving |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Haalt het wachtwoord op dat wordt gebruikt om items te ontsleutelen. |
| [getEncoding()](#getEncoding--) | Haalt de codering op die wordt gebruikt voor itemnamen. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | Haalt op of checksum‑verificatie van ALZ‑items wordt overgeslagen. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Stelt een annuleringsvlag in die wordt gebruikt om extractie te annuleren. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Stelt het wachtwoord in dat wordt gebruikt om items te ontsleutelen. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Stelt de codering in die wordt gebruikt voor itemnamen. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | Stelt in of checksum‑verificatie van ALZ‑items wordt overgeslagen. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Haalt het wachtwoord op dat wordt gebruikt om items te ontsleutelen.

**Returns:**
java.lang.String - wachtwoord dat wordt gebruikt om items te ontsleutelen, of `null` wanneer er geen is geconfigureerd
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Haalt de codering op die wordt gebruikt voor itemnamen. Standaard is Koreaanse Windows‑codepagina 949 (CP949). ALZ‑archieven slaan historisch gezien bestandsnamen op met de Koreaanse Windows ANSI‑codepagina.

**Returns:**
java.nio.charset.Charset - codering die wordt gebruikt voor itemnamen
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


Haalt op of checksum‑verificatie van ALZ‑items wordt overgeslagen. Standaard is `false`.

**Returns:**
boolean - of checksum‑verificatie wordt overgeslagen
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Stelt een annuleringsvlag in die wordt gebruikt om extractie te annuleren.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | annuleringsvlag, of `null` om annulering uit te schakelen |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Stelt het wachtwoord in dat wordt gebruikt om items te ontsleutelen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | wachtwoord dat wordt gebruikt om items te ontsleutelen |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Stelt de codering in die wordt gebruikt voor itemnamen. ALZ‑archieven slaan historisch gezien bestandsnamen op met de Koreaanse Windows ANSI‑codepagina.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.nio.charset.Charset | codering die wordt gebruikt voor itemnamen |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


Stelt in of checksum‑verificatie van ALZ‑items wordt overgeslagen.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | of checksum‑verificatie wordt overgeslagen |

