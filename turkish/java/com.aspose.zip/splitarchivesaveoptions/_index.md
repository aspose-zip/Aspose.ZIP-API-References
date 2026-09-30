---
title: "SplitArchiveSaveOptions"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Çok bölümlü ZIP arşivi kaydetme seçenekleri."
type: docs
weight: 122
url: /tr/java/com.aspose.zip/splitarchivesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public class SplitArchiveSaveOptions
```

Çok bölümlü ZIP arşivi kaydetme seçenekleri.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SplitArchiveSaveOptions(String fileName, long segmentSize)](#SplitArchiveSaveOptions-java.lang.String-long-) | Çok bölümlü ZIP arşivi kaydetmek için ayarları oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getArchiveComment()](#getArchiveComment--) | Zip dosyası için isteğe bağlı yorumu alır. |
| [getCloseEntrySource()](#getCloseEntrySource--) | Bir girdinin sıkıştırılmasının hemen ardından girdilerin kaynaklarının kapatılıp kapatılmayacağını gösteren değeri alır. |
| [getEncoding()](#getEncoding--) | Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlamayı alır. |
| [getEventsBag()](#getEventsBag--) | Arşiv kaydedilirken tetiklenen olayların konteynerini alır. |
| [getFileName()](#getFileName--) | Uzantısız segmentlerin adını alır. |
| [getSegmentSize()](#getSegmentSize--) | Segmentin boyutunu alır. |
| [setArchiveComment(String value)](#setArchiveComment-java.lang.String-) | Zip dosyası için isteğe bağlı yorumu ayarlar. |
| [setCloseEntrySource(boolean value)](#setCloseEntrySource-boolean-) | Bir giriş sıkıştırıldıktan hemen sonra girişlerin kaynaklarının kapatılıp kapanmayacağını belirten bir değer ayarlar. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlamayı ayarlar. |
| [setEventsBag(EventsBag value)](#setEventsBag-com.aspose.zip.EventsBag-) | Arşiv kaydedilirken tetiklenen olayların konteynerini ayarlar. |
### SplitArchiveSaveOptions(String fileName, long segmentSize) {#SplitArchiveSaveOptions-java.lang.String-long-}
```
public SplitArchiveSaveOptions(String fileName, long segmentSize)
```


Çok bölümlü ZIP arşivi kaydetmek için ayarları oluşturur.

Bazı bölümler `segmentSize` değerinden daha küçük olabilir. Çoğu durumda, son segment daha küçük olur ancak nadiren normal segmentler de çok küçük olabilir.

Dosya adları şu şekilde olacaktır: `fileName`.z01, `fileName`.z02, ..., `fileName`.z(n-1), `fileName`.zip.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Bölümler için ad. .zip uzantısı ile ya da olmadan olabilir. |
| segmentSize | long | Bölümün boyutu. |

### getArchiveComment() {#getArchiveComment--}
```
public final String getArchiveComment()
```


Zip dosyası için isteğe bağlı yorumu alır.

**Returns:**
java.lang.String - Zip dosyası için isteğe bağlı yorum.
### getCloseEntrySource() {#getCloseEntrySource--}
```
public final boolean getCloseEntrySource()
```


Bir girdinin sıkıştırılmasının hemen ardından girdilerin kaynaklarının kapatılıp kapatılmayacağını gösteren değeri alır.

**Returns:**
boolean - Bir giriş sıkıştırıldıktan hemen sonra girişlerin kaynaklarının kapatılıp kapanmayacağını belirten bir değer.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlamayı alır.

Ayarlanmamışsa, kod sayfası 437 kullanılacaktır.

**Returns:**
java.nio.charset.Charset - Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlama.
### getEventsBag() {#getEventsBag--}
```
public final EventsBag getEventsBag()
```


Arşiv kaydedilirken tetiklenen olayların konteynerini alır.

**Returns:**
[EventsBag](../../com.aspose.zip/eventsbag) - container of events raising on archive saving.
### getFileName() {#getFileName--}
```
public final String getFileName()
```


Uzantısız segmentlerin adını alır.

**Returns:**
java.lang.String - uzantısız segmentlerin adı.
### getSegmentSize() {#getSegmentSize--}
```
public final long getSegmentSize()
```


Segmentin boyutunu alır.

**Returns:**
long - segmentin boyutu.
### setArchiveComment(String value) {#setArchiveComment-java.lang.String-}
```
public final void setArchiveComment(String value)
```


Zip dosyası için isteğe bağlı yorumu ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Zip dosyası için isteğe bağlı yorum. |

### setCloseEntrySource(boolean value) {#setCloseEntrySource-boolean-}
```
public final void setCloseEntrySource(boolean value)
```


Bir giriş sıkıştırıldıktan hemen sonra girişlerin kaynaklarının kapatılıp kapanmayacağını belirten bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir girişin kaynaklarının sıkıştırıldıktan hemen sonra kapatılıp kapatılmayacağını gösteren değer. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlamayı ayarlar.

Ayarlanmamışsa, kod sayfası 437 kullanılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.nio.charset.Charset | Dosya adlarını ve diğer dizeleri baytlara dönüştürmek için kodlama. |

### setEventsBag(EventsBag value) {#setEventsBag-com.aspose.zip.EventsBag-}
```
public final void setEventsBag(EventsBag value)
```


Arşiv kaydedilirken tetiklenen olayların konteynerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [EventsBag](../../com.aspose.zip/eventsbag) | Arşiv kaydedilirken tetiklenen olayların konteyneri. |

