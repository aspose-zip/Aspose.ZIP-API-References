---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP voor Java API-referentie"
description: "Basisklasse voor instellingen voor verschillende 7z-encryptiemethoden."
type: docs
weight: 112
url: /nl/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Basisklasse voor instellingen voor verschillende 7z-encryptiemethoden.

De AES-256 is de enige mogelijke encryptiemethode voor een 7z-archief. Dus de [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) is de enige implementatie.
## Methoden

| Methode | Beschrijving |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Haalt een waarde op die aangeeft of de header versleuteld is. |
| [getPassword()](#getPassword--) | Haalt het wachtwoord op voor versleuteling of ontsleuteling. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Stelt een waarde in die aangeeft of de header versleuteld is. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Stelt het wachtwoord in voor versleuteling of ontsleuteling. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Haalt een waarde op die aangeeft of de header versleuteld is.

Deze instelling is gelijk aan de `-mhe=on` schakelaar van het 7-Zip‑hulpmiddel. Momenteel is deze niet compatibel met headercompressie.

**Returns:**
boolean - een waarde die aangeeft of de header versleuteld is
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Haalt het wachtwoord op voor versleuteling of ontsleuteling.

**Returns:**
java.lang.String - wachtwoord voor versleuteling of ontsleuteling
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Stelt een waarde in die aangeeft of de header versleuteld is.

Deze instelling is gelijk aan de `-mhe=on` schakelaar van het 7-Zip‑hulpmiddel. Momenteel is deze niet compatibel met headercompressie.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | boolean | een waarde die aangeeft of de header versleuteld is |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Stelt het wachtwoord in voor versleuteling of ontsleuteling.

**Parameters:**
| Parameter | Type | Beschrijving |
| --- | --- | --- |
| waarde | java.lang.String | wachtwoord voor versleuteling of ontsleuteling |

