---
title: "CancelEntryEventArgs"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "रद्द करने योग्य प्रविष्टि संबंधित घटनाओं के लिए इवेंट तर्क।"
type: docs
weight: 52
url: /hi/java/com.aspose.zip/cancelentryeventargs/
---

**Inheritance:**
java.lang.Object, com.aspose.ms.System.EventArgs, [com.aspose.zip.EntryEventArgs](../../com.aspose.zip/entryeventargs)
```
public class CancelEntryEventArgs extends EntryEventArgs
```

रद्द करने योग्य प्रविष्टि संबंधित घटनाओं के लिए इवेंट तर्क।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [CancelEntryEventArgs(ArchiveEntry entry)](#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-) | नए [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) क्लास का एक नया उदाहरण प्रारंभ करता है। |
## Methods

| Method | विवरण |
| --- | --- |
| [getCancel()](#getCancel--) | एक मान प्राप्त करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं। |
| [setCancel(boolean value)](#setCancel-boolean-) | एक मान सेट करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं। |
### CancelEntryEventArgs(ArchiveEntry entry) {#CancelEntryEventArgs-com.aspose.zip.ArchiveEntry-}
```
public CancelEntryEventArgs(ArchiveEntry entry)
```


नए [CancelEntryEventArgs](../../com.aspose.zip/cancelentryeventargs) क्लास का एक नया उदाहरण प्रारंभ करता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| entry | [ArchiveEntry](../../com.aspose.zip/archiveentry) | इवेंट जिस आर्काइव एंट्री के लिए उठाया गया है। |

### getCancel() {#getCancel--}
```
public final boolean getCancel()
```


एक मान प्राप्त करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं।

**Returns:**
boolean - true यदि इवेंट को रद्द किया जाना चाहिए; अन्यथा false।
### setCancel(boolean value) {#setCancel-boolean-}
```
public final void setCancel(boolean value)
```


एक मान सेट करता है जो दर्शाता है कि इवेंट को रद्द किया जाना चाहिए या नहीं।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | बूलियन | true यदि इवेंट को रद्द किया जाना चाहिए; अन्यथा false. |

