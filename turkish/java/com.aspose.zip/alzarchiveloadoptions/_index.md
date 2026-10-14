---
title: "AlzArchiveLoadOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Bir ALZ arşivin sıkıştırılmış bir dosyadan yüklendiği seçenekler."
type: docs
weight: 12
url: /tr/java/com.aspose.zip/alzarchiveloadoptions/
---

**Inheritance:**
java.lang.Object
```
public class AlzArchiveLoadOptions
```

Bir ALZ arşivin sıkıştırılmış bir dosyadan yüklendiği seçenekler.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [AlzArchiveLoadOptions()](#AlzArchiveLoadOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getDecryptionPassword()](#getDecryptionPassword--) | Girişleri çözmek için kullanılan şifreyi alır. |
| [getEncoding()](#getEncoding--) | Giriş adları için kullanılan kodlamayı alır. |
| [getSkipChecksumVerification()](#getSkipChecksumVerification--) | ALZ girişlerinin sağlama kontrolünün atlanıp atlanmadığını alır. |
| [setCancellationFlag(CancellationFlag value)](#setCancellationFlag-com.aspose.zip.CancellationFlag-) | Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar. |
| [setDecryptionPassword(String value)](#setDecryptionPassword-java.lang.String-) | Girişleri çözmek için kullanılan şifreyi ayarlar. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Giriş adları için kullanılan kodlamayı ayarlar. |
| [setSkipChecksumVerification(boolean value)](#setSkipChecksumVerification-boolean-) | ALZ girişlerinin sağlama kontrolünün atlanıp atlanmayacağını ayarlar. |
### AlzArchiveLoadOptions() {#AlzArchiveLoadOptions--}
```
public AlzArchiveLoadOptions()
```


### getDecryptionPassword() {#getDecryptionPassword--}
```
public String getDecryptionPassword()
```


Girişleri çözmek için kullanılan şifreyi alır.

**Returns:**
java.lang.String - girişleri çözmek için kullanılan şifre, ya da hiçbir şey yapılandırılmadığında `null`
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Giriş adları için kullanılan kodlamayı alır. Varsayılan, Kore Windows kod sayfası 949 (CP949)'dir. ALZ arşivleri tarihsel olarak dosya adlarını Kore Windows ANSI kod sayfasını kullanarak depolar.

**Returns:**
java.nio.charset.Charset - giriş adları için kullanılan kodlama
### getSkipChecksumVerification() {#getSkipChecksumVerification--}
```
public boolean getSkipChecksumVerification()
```


ALZ girişlerinin sağlama kontrolünün atlanıp atlanmadığını alır. Varsayılan `false`.

**Returns:**
boolean - sağlama kontrolünün atlanıp atlanmadığı
### setCancellationFlag(CancellationFlag value) {#setCancellationFlag-com.aspose.zip.CancellationFlag-}
```
public void setCancellationFlag(CancellationFlag value)
```


Çıkarma işlemini iptal etmek için kullanılan bir iptal bayrağı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CancellationFlag](../../com.aspose.zip/cancellationflag) | iptal bayrağı, veya iptali devre dışı bırakmak için `null` |

### setDecryptionPassword(String value) {#setDecryptionPassword-java.lang.String-}
```
public void setDecryptionPassword(String value)
```


Girişleri çözmek için kullanılan şifreyi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | girişleri çözmek için kullanılan şifre |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Giriş adları için kullanılan kodlamayı ayarlar. ALZ arşivleri tarihsel olarak dosya adlarını Kore Windows ANSI kod sayfası kullanarak depolar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.nio.charset.Charset | giriş adları için kullanılan kodlama |

### setSkipChecksumVerification(boolean value) {#setSkipChecksumVerification-boolean-}
```
public void setSkipChecksumVerification(boolean value)
```


ALZ girişlerinin sağlama kontrolünün atlanıp atlanmayacağını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | kontrol toplamı doğrulamasının atlanıp atlanmadığı |

