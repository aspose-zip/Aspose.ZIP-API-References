---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP for Java API Referansı"
description: "İptal edilebilir girişle ilgili olaylar için olay argümanları."
type: docs
weight: 52
url: /tr/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

İptal edilebilir girişle ilgili olaylar için olay argümanları.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | Yeni bir [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCancel()](#getCancel--) | Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri alır. |
| [setCancel(boolean value)](#setCancel-boolean-) | Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri ayarlar. |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


Yeni bir [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Olayın tetiklendiği arşiv girdisi. |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri alır.

**Returns:**
boolean - olay iptal edilmesi gerekiyorsa true; aksi takdirde false.
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


Olayın iptal edilip edilmemesi gerektiğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | olay iptal edilmesi gerekiyorsa true; aksi takdirde false. |

