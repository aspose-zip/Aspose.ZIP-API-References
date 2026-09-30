---
title: "UueSaveOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Uuencoded dosya kaydetme seçenekleri."
type: docs
weight: 129
url: /tr/java/com.aspose.zip/uuesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class UueSaveOptions
```

Uuencoded dosya kaydetme seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [UueSaveOptions(String fileName, String newLine)](#UueSaveOptions-java.lang.String-java.lang.String-) | Seçenekleri, kullanıcı tarafından sağlanan dosya adı ve yeni satır ile başlatır. |
| [UueSaveOptions(String fileName)](#UueSaveOptions-java.lang.String-) | Seçenekleri, kullanıcı tarafından sağlanan dosya adı ve varsayılan yeni satır ile başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getFileName()](#getFileName--) | Kod çözülmüş veriyi yeniden oluştururken kullanılacak dosya adını alır. |
| [getNewLine()](#getNewLine--) | Her satırı sonlandıran karakteri alır, genellikle "\n" veya "\r\n". |
| [getUnixFilePermissions()](#getUnixFilePermissions--) | Dosyanın Unix dosya izinlerini alır. |
| [setUnixFilePermissions(String value)](#setUnixFilePermissions-java.lang.String-) | Dosyanın Unix dosya izinlerini ayarlar. |
### UueSaveOptions(String fileName, String newLine) {#UueSaveOptions-java.lang.String-java.lang.String-}
```
public UueSaveOptions(String fileName, String newLine)
```


Seçenekleri, kullanıcı tarafından sağlanan dosya adı ve yeni satır ile başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | kod çözülmüş veriyi yeniden oluştururken kullanılacak dosya adı |
| newLine | java.lang.String | her satırı sonlandıran karakter |

### UueSaveOptions(String fileName) {#UueSaveOptions-java.lang.String-}
```
public UueSaveOptions(String fileName)
```


Seçenekleri, kullanıcı tarafından sağlanan dosya adı ve varsayılan yeni satır ile başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | kod çözülmüş veriyi yeniden oluştururken kullanılacak dosya adı |

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Kod çözülmüş veriyi yeniden oluştururken kullanılacak dosya adını alır.

**Returns:**
java.lang.String - kod çözülmüş veriyi yeniden oluştururken kullanılacak dosya adı
### getNewLine() {#getNewLine--}
```
public final String getNewLine()
```


Her satırı sonlandıran karakteri alır, genellikle "\n" veya "\r\n".

**Returns:**
java.lang.String - her satırı sonlandıran karakter, genellikle "\n" veya "\r\n".
### getUnixFilePermissions() {#getUnixFilePermissions--}
```
public final String getUnixFilePermissions()
```


Dosyanın Unix dosya izinlerini alır.

Varsayılan 644'tür.

**Returns:**
java.lang.String - dosyanın Unix dosya izinleri
### setUnixFilePermissions(String value) {#setUnixFilePermissions-java.lang.String-}
```
public final void setUnixFilePermissions(String value)
```


Dosyanın Unix dosya izinlerini ayarlar.

Varsayılan 644'tür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | dosyanın Unix dosya izinleri |

