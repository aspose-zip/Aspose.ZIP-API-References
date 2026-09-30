---
title: "LzipLoadOptions.CancellationToken"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "LzipLoadOptions प्रॉपर्टी। एक्सट्रैक्शन ऑपरेशन को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन टोकन को प्राप्त या सेट करता है।"
type: docs
weight: 20
url: /hi/net/aspose.zip.lzip/lziploadoptions/cancellationtoken/
---
## LzipLoadOptions.CancellationToken property

निकालने की प्रक्रिया को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन टोकन को प्राप्त करता है या सेट करता है।

```csharp
public CancellationToken CancellationToken { get; set; }
```

## टिप्पणियाँ

यह प्रॉपर्टी .NET Framework 4.0 और उससे ऊपर के संस्करणों के लिए मौजूद है।

## उदाहरण

एक निश्चित समय के बाद lzip आर्काइव निष्कर्षण को रद्द करें।

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new LzipArchive("big.lz", new LzipLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.Extract("data.bin");
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
    var loadOptions = new LzipLoadOptions() { CancellationToken = cts.Token };
    using (var a = LzipArchive("big.lz", loadOptions))
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

* class [LzipLoadOptions](../)
* namespace [Aspose.Zip.Lzip](../../lziploadoptions/)
* assembly [Aspose.Zip](../../../)


