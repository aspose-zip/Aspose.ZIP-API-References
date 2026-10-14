---
title: "ProgressCancelEventArgs"
second_title: "Aspose.ZIP for Java API Referansı"
description: "İptal edilebilir olay verileri, işlenen bayt sayısını içeren sınıf."
type: docs
weight: 95
url: /tr/java/com.aspose.zip/progresscanceleventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.ProgressEventArgs](../../com.aspose.zip/progresseventargs)
```
public class ProgressCancelEventArgs extends ProgressEventArgs
```

İptal edilebilir olay verileri, işlenen bayt sayısını içeren sınıf.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ProgressCancelEventArgs(long proceededBytes)](#ProgressCancelEventArgs-long-) | Yeni bir [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCancel()](#getCancel--) | Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri alır. |
| [setCancel(boolean value)](#setCancel-boolean-) | Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri ayarlar. |
### ProgressCancelEventArgs(long proceededBytes) {#ProgressCancelEventArgs-long-}
```
public ProgressCancelEventArgs(long proceededBytes)
```


Yeni bir [ProgressCancelEventArgs](../../com.aspose.zip/progresscanceleventargs) sınıfının örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| proceededBytes | long | İşlenen bayt sayısı. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri alır.

**Returns:**
boolean - Olay iptal edilmeliyse True; aksi takdirde false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | olayın iptal edilip edilmeyeceğini gösteren bir değer. |

