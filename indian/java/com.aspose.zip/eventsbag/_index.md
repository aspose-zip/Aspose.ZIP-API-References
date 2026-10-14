---
title: "EventsBag"
second_title: "Aspose.ZIP जावा API रेफ़रेंस"
description: "सहेजने पर उपयोग किया जाने वाला इवेंट कंटेनर।"
type: docs
weight: 65
url: /hi/java/com.aspose.zip/eventsbag/
---

**Inheritance:**
java.lang.Object
```
public final class EventsBag
```

इवेंट्स कंटेनर का उपयोग [Archive](../../com.aspose.zip/archive) सहेजने पर किया जाता है।
## कंस्ट्रक्टर

| कंस्ट्रक्टर | विवरण |
| --- | --- |
| [EventsBag()](#EventsBag--) |  |
## Methods

| Method | विवरण |
| --- | --- |
| [getEntryAccessed()](#getEntryAccessed--) | एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है। |
| [getEntryCompressed()](#getEntryCompressed--) | एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है। |
| [setEntryAccessed(Event&lt;EntryEventArgs&gt; value)](#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--) | एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है। |
| [setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value)](#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--) | एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है। |
### EventsBag() {#EventsBag--}
```
public EventsBag()
```


### getEntryAccessed() {#getEntryAccessed--}
```
public Event<EntryEventArgs> getEntryAccessed()
```


एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है।

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised before an archive entry is being compressed
### getEntryCompressed() {#getEntryCompressed--}
```
public Event<CancelEntryEventArgs> getEntryCompressed()
```


एक इवेंट प्राप्त करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है।

**Returns:**
[Event](../../com.aspose.zip/event) - an event that is raised after an archive entry has been compressed
### setEntryAccessed(Event&lt;EntryEventArgs&gt; value) {#setEntryAccessed-com.aspose.zip.Event-com.aspose.zip.EntryEventArgs--}
```
public void setEntryAccessed(Event<EntryEventArgs> value)
```


एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने से पहले उत्पन्न होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.EntryEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब एक आर्काइव एंट्री को संपीड़ित किया जा रहा हो। |

### setEntryCompressed(Event&lt;CancelEntryEventArgs&gt; value) {#setEntryCompressed-com.aspose.zip.Event-com.aspose.zip.CancelEntryEventArgs--}
```
public void setEntryCompressed(Event<CancelEntryEventArgs> value)
```


एक इवेंट सेट करता है जो आर्काइव प्रविष्टि के संपीड़ित होने के बाद उत्पन्न होता है।

**Parameters:**
| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| मान | com.aspose.zip.Event&lt;com.aspose.zip.CancelEntryEventArgs&gt; | एक इवेंट जो तब उठाया जाता है जब एक आर्काइव एंट्री संपीड़ित हो चुकी होती है। |

