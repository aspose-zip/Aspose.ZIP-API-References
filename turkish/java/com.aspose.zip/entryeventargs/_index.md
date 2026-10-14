---
title: "EntryEventArgs"
second_title: "Aspose.ZIP for Java API Referansı"
description: "Girişle ilgili olaylar için olay argümanları."
type: docs
weight: 62
url: /tr/java/com.aspose.zip/entryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs
```
public class EntryEventArgs extends System.EventArgs
```

Girişle ilgili olaylar için olay argümanları.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [EntryEventArgs(ArchiveEntry entry)](#EntryEventArgs-com.aspose.zip.ArchiveEntry-) | Yeni bir [EntryEventArgs](../../com.aspose.zip/entryeventargs) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getEntry()](#getEntry--) | Olayın tetiklendiği arşiv girdisini alır. |
### EntryEventArgs(ArchiveEntry entry) {#EntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public EntryEventArgs(ArchiveEntry entry)
```


Yeni bir [EntryEventArgs](../../com.aspose.zip/entryeventargs) sınıfı örneği başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | Olayın tetiklendiği arşiv girdisi. |

### getEntry() {#getEntry--}
```
public final ArchiveEntry getEntry()
```


Olayın tetiklendiği arşiv girdisini alır.

**Returns:**
[ArchiveEntry](../../com.aspose.zip/archiveentry) - the archive entry the event is raised for.
