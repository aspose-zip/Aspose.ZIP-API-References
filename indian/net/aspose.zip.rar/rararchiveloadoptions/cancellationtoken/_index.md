---
title: "RarArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "RarArchiveLoadOptions प्रॉपर्टी। निष्कर्षण ऑपरेशन को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन टोकन को प्राप्त या सेट करता है"
type: docs
weight: 20
url: /hi/net/aspose.zip.rar/rararchiveloadoptions/cancellationtoken/
---
## RarArchiveLoadOptions.CancellationToken property

निकालने की प्रक्रिया को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन टोकन को प्राप्त करता है या सेट करता है।

```csharp
public CancellationToken CancellationToken { get; set; }
```

## टिप्पणियाँ

यह प्रॉपर्टी .NET Framework 4.0 और उससे ऊपर के संस्करणों के लिए मौजूद है।

## उदाहरण

किसी निश्चित समय के बाद RAR आर्काइव निष्कर्षण रद्द करें।

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new RarArchive("big.rar", new RarArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.Entries[0].Extract("data.bin");
        }
        catch(OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

`Task` के साथ उपयोग करना

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new RarArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = new RarArchive("big.rar", loadOptions))
    {
         a.ExtractToDirectory("destination");
    }
}, cts.Token);

t.ContinueWith(delegate(Task antecedent)
{
     if (antecedent.IsCanceled)
     {
         Console.WriteLine("Extraction was cancelled after 60 seconds");
     }

     cts.Dispose();
});
```

रद्दीकरण के कारण अधिकांशतः कुछ डेटा एक्सट्रैक्ट नहीं होता।

### संबंधित देखें

* class [RarArchiveLoadOptions](../)
* namespace [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


