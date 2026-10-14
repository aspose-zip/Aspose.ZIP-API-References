---
title: "IsoLoadOptions.EntryExtractionProgressed"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "IsoLoadOptions प्रॉपर्टी। जब कुछ बाइट्स एक्सट्रैक्ट हो जाएँ तो कॉल होने वाले डेलीगेट को प्राप्त या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.iso/isoloadoptions/entryextractionprogressed/
---
## IsoLoadOptions.EntryExtractionProgressed property

जब कुछ बाइट्स निकाले जा चुके हों तो बुलाए जाने वाले डेलीगेट को प्राप्त करता है या सेट करता है।

```csharp
public EventHandler<ProgressEventArgs> EntryExtractionProgressed { get; set; }
```

## टिप्पणियाँ

इवेंट भेजने वाला वह [`IsoEntry`](../../isoentry/) इंस्टेंस है जिसका एक्सट्रैक्शन प्रोग्रेस हो रहा है।

## उदाहरण

```csharp
IsoArchive archive = new IsoArchive("archive.iso", 
new IsoLoadOptions() { EntryExtractionProgressed = (s, e) => { int percent = (int)((100 * e.ProceededBytes) / length); } })                 
```

### संबंधित देखें

* class [ProgressEventArgs](../../../aspose.zip/progresseventargs/)
* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


