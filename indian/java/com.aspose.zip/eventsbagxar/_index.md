---
title: "EventsBagXar"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "सहेजने पर उपयोग किया जाने वाला इवेंट कंटेनर।"
type: docs
weight: 67
url: /hi/java/com.aspose.zip/eventsbagxar/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBagXar
```

सहेजने पर [XarArchive](../../com.aspose.zip/xararchive) में उपयोग किया जाने वाला इवेंट कंटेनर।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [EventsBagXar()](#EventsBagXar--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है। |
| [getEntryCompressed()](#getEntryCompressed--) | एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है। |
| [setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--) | एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है। |
| [setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--) | एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है। |
### EventsBagXar() {#EventsBagXar--}
```
public EventsBagXar()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgsXar> getEntryAccessed()
```


एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है।

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgsXar> getEntryCompressed()
```


एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है।

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgsXar&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgsXar--}
```
public void setEntryAccessed(Event<EntryEventArgsXar> value)
```


एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgsXar&gt; | एक इवेंट जो तब उठाया जाता है जब एक आर्काइव एंट्री को संपीड़ित किया जा रहा हो। |

### setEntryCompressed(Event&lt;CancelEntryEventArgsXar&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgsXar--}
```
public void setEntryCompressed(Event<CancelEntryEventArgsXar> value)
```


एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgsXar&gt; | एक इवेंट जो तब उठाया जाता है जब एक आर्काइव एंट्री संपीड़ित हो चुकी होती है। |

