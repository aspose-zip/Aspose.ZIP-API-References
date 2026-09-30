---
title: "SevenZipEncryptionSettings"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Birçok 7z şifreleme yöntemi için ayarların temel sınıfı."
type: docs
weight: 112
url: /tr/java/com.aspose.zip/sevenzipencryptionsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class SevenZipEncryptionSettings
```

Birçok 7z şifreleme yöntemi için ayarların temel sınıfı.

AES-256, 7z arşivi için mevcut tek şifreleme yöntemidir. Bu nedenle [SevenZipAESEncryptionSettings](../../com.aspose.zip/sevenzipaesencryptionsettings) tek uygulamadır.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getEncryptHeader()](#getEncryptHeader--) | Üstbilgi şifrelemesini gösteren bir değeri alır. |
| [getPassword()](#getPassword--) | Şifreleme veya şifre çözme için parolayı alır. |
| [setEncryptHeader(boolean value)](#setEncryptHeader-boolean-) | Üstbilgi şifrelemesini gösteren bir değeri ayarlar. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Şifreleme veya şifre çözme için parolayı ayarlar. |
### getEncryptHeader() {#getEncryptHeader--}
```
public final boolean getEncryptHeader()
```


Üstbilgi şifrelemesini gösteren bir değeri alır.

Bu ayar, 7-Zip aracının `-mhe=on` anahtarına eşdeğerdir. Şu anda, üstbilgi sıkıştırmasıyla uyumsuzdur.

**Returns:**
boolean - üstbilgi şifrelemesini gösteren bir değer
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Şifreleme veya şifre çözme için parolayı alır.

**Returns:**
java.lang.String - şifreleme veya şifre çözme için parola
### setEncryptHeader(boolean value) {#setEncryptHeader-boolean-}
```
public final void setEncryptHeader(boolean value)
```


Üstbilgi şifrelemesini gösteren bir değeri ayarlar.

Bu ayar, 7-Zip aracının `-mhe=on` anahtarına eşdeğerdir. Şu anda, üstbilgi sıkıştırmasıyla uyumsuzdur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | üstbilgi şifrelemesini gösteren bir değer |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Şifreleme veya şifre çözme için parolayı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | şifreleme veya şifre çözme için parola |

