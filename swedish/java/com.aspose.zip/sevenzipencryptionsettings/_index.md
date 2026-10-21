---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP för Java API-referens"
description: "Bas-klass för inställningar för flera 7z-krypteringsmetoder."
type: docs
weight: 112
url: /sv/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Bas-klass för inställningar för flera 7z-krypteringsmetoder.

Den AES-256 är den enda möjliga krypteringsmetoden för 7z-arkivet. Så [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) är den enda implementeringen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Hämtar ett värde som indikerar rubrikkryptering. |
| [getPassword()](#getPassword--) | Hämtar lösenord för kryptering eller avkryptering. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Ställer in ett värde som indikerar rubrikkryptering. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Ställer in lösenord för kryptering eller avkryptering. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Hämtar ett värde som indikerar rubrikkryptering.

Denna inställning motsvarar `-mhe=on`-växeln i 7-Zip-verktyget. För närvarande är den inkompatibel med rubrikkomprimering.

**Returns:**
boolean - ett värde som indikerar rubrikkryptering
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Hämtar lösenord för kryptering eller avkryptering.

**Returns:**
java.lang.String - lösenord för kryptering eller avkryptering
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Ställer in ett värde som indikerar rubrikkryptering.

Denna inställning motsvarar `-mhe=on`-växeln i 7-Zip-verktyget. För närvarande är den inkompatibel med rubrikkomprimering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean | ett värde som indikerar rubrikkryptering |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Ställer in lösenord för kryptering eller avkryptering.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String | lösenord för kryptering eller avkryptering |

