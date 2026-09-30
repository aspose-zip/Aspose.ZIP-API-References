---
title: "WimLoadOptions.CancellationToken"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "WimLoadOptions प्रॉपर्टी। प्राप्त करता है या सेट करता है एक cancellation token जिसका उपयोग extraction operation को रद्द करने के लिए किया जाता है।"
type: docs
weight: 20
url: /hi/net/aspose.zip.wim/wimloadoptions/cancellationtoken/
---
## WimLoadOptions.CancellationToken property

निकालने की प्रक्रिया को रद्द करने के लिए उपयोग किए जाने वाले कैंसलेशन टोकन को प्राप्त करता है या सेट करता है।

```csharp
public CancellationToken CancellationToken { get; set; }
```

## टिप्पणियाँ

यह प्रॉपर्टी .NET Framework 4.0 और उससे ऊपर के संस्करणों के लिए मौजूद है।

## उदाहरण

एक निश्चित समय के बाद WIM आर्काइव extraction को रद्द करें।

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new WimArchive("big.wim", new WimLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
            a.Images[0].AllEntries.OfType<WimFileEntry>().First().Extract("data.bin");
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
    var loadOptions = new WimLoadOptions() { CancellationToken = cts.Token };
    using (var a = WimArchive("big.wim", loadOptions))
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

* class [WimLoadOptions](../)
* namespace [Aspose.Zip.Wim](../../wimloadoptions/)
* assembly [Aspose.Zip](../../../)


