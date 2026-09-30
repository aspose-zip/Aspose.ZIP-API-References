---
title: "AppleArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AppleArchiveLoadOptions प्रॉपर्टी। निष्कर्षण ऑपरेशन को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन टोकन को प्राप्त या सेट करता है"
type: docs
weight: 20
url: /hi/net/aspose.zip.apple/applearchiveloadoptions/cancellationtoken/
---
## AppleArchiveLoadOptions.CancellationToken property

निकालने की प्रक्रिया को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन टोकन को प्राप्त करता है या सेट करता है।

```csharp
public CancellationToken CancellationToken { get; set; }
```

## टिप्पणियाँ

यह प्रॉपर्टी .NET Framework 4.0 और उससे ऊपर के संस्करणों के लिए मौजूद है।

## उदाहरण

किसी निश्चित समय के बाद Apple Archive निष्कर्षण को रद्द करें।

```csharp
using (System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource())
{
    cts.CancelAfter(System.TimeSpan.FromSeconds(60)); 
    using (var a = new AppleArchive("big.aar", new AppleArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.ExtractToDirectory("destination");
        }
        catch(System.OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

`Task` के साथ उपयोग करना

```csharp
System.Threading.CancellationTokenSource cts = new System.Threading.CancellationTokenSource();
cts.CancelAfter(System.TimeSpan.FromSeconds(60));
System.Threading.Tasks.Task t = System.Threading.Tasks.Task.Run(delegate()
{
    var loadOptions = new AppleArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = new AppleArchive("big.aar", loadOptions))
    {
         a.ExtractToDirectory("destination");
    }
}, cts.Token);

t.ContinueWith(delegate(System.Threading.Tasks.Task antecedent)
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

* class [AppleArchiveLoadOptions](../)
* namespace [Aspose.Zip.Apple](../../applearchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


