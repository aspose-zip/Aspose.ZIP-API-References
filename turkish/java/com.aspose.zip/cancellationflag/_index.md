---
title: "CancellationFlag"
second_title: "Aspose.ZIP for Java API Referansı"
description: "İşlemlerin iptaline izin veren bayrak."
type: docs
weight: 54
url: /tr/java/com.aspose.zip/cancellationflag/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.AutoCloseable
```
public class CancellationFlag implements AutoCloseable
```

İşlemlerin iptaline izin veren bayrak.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CancellationFlag()](#CancellationFlag--) | Bir CancellationFlag örneği oluşturur. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [cancel()](#cancel--) | Bu [CancellationFlag](../../com.aspose.zip/cancellationflag) örneğiyle ilişkili işlemi iptal eder. |
| [cancelAfter(long delay)](#cancelAfter-long-) | Belirtilen milisaniye gecikmesinden sonra işlemi iptal eder. |
| [cancelAfter(long delay, TimeUnit unit)](#cancelAfter-long-java.util.concurrent.TimeUnit-) | Belirtilen gecikmeden sonra, verilen zaman biriminde işlemi iptal eder. |
| [close()](#close--) | [CancellationFlag](../../com.aspose.zip/cancellationflag) örneğini kapatır ve ona bağlı tüm kaynakları serbest bırakır. |
### CancellationFlag() {#CancellationFlag--}
```
public CancellationFlag()
```


Bir CancellationFlag örneği oluşturur.

### cancel() {#cancel--}
```
public void cancel()
```


Bu [CancellationFlag](../../com.aspose.zip/cancellationflag) örneğiyle ilişkili işlemi iptal eder.

İşlem zaten iptal edilmişse, bu yöntem hiçbir şey yapmaz.

### cancelAfter(long delay) {#cancelAfter-long-}
```
public void cancelAfter(long delay)
```


Belirtilen milisaniye gecikmesinden sonra işlemi iptal eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gecikme | long | İşlemin iptal edileceği milisaniye cinsinden gecikme. |

### cancelAfter(long delay, TimeUnit unit) {#cancelAfter-long-java.util.concurrent.TimeUnit-}
```
public void cancelAfter(long delay, TimeUnit unit)
```


Belirtilen gecikmeden sonra, verilen zaman biriminde işlemi iptal eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gecikme | long | İşlemin iptal edileceği gecikme. |
| birim | java.util.concurrent.TimeUnit | Gecikme parametresinin zaman birimi. |

### close() {#close--}
```
public void close()
```


[CancellationFlag](../../com.aspose.zip/cancellationflag) örneğini kapatır ve ona bağlı tüm kaynakları serbest bırakır.

