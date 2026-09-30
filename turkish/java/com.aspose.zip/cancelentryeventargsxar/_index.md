---
title: "CancelEntryEventArgsXar"
second_title: "Aspose.ZIP for Java API Referansı"
description: "İptal edilebilir girişle ilgili olaylar için olay argümanları."
type: docs
weight: 53
url: /tr/java/com.aspose.zip/cancelentryeventargsxar/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgsXar](../../com.aspose.zip/entryeventargsxar)
```
public class CancelEntryEventArgsXar extends EntryEventArgsXar
```

İptal edilebilir girişle ilgili olaylar için olay argümanları.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CancelEntryEventArgsXar(XarEntry entry)](#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-) | Yeni bir [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCancel()](#getCancel--) | Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri alır. |
| [setCancel(boolean value)](#setCancel-boolean-) | Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri ayarlar. |
### CancelEntryEventArgsXar(XarEntry entry) {#CancelEntryEventArgsXar-com.aspose.zip.XarEntry-}
```
public CancelEntryEventArgsXar(XarEntry entry)
```


Yeni bir [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| entry | [XarEntry](../../com.aspose.zip/xarentry) | olayın yükseltildiği arşiv girdisi |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri alır.

**Returns:**
boolean - olay iptal edilmeliyse true; aksi takdirde false
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | olay iptal edilmeliyse true; aksi takdirde false |

