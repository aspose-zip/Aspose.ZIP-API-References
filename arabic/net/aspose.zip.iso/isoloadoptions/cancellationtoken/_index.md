---
title: "IsoLoadOptions.CancellationToken"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية IsoLoadOptions. تحصل أو تعين رمز إلغاء يُستخدم لإلغاء عملية الاستخراج"
type: docs
weight: 20
url: /ar/net/aspose.zip.iso/isoloadoptions/cancellationtoken/
---
## IsoLoadOptions.CancellationToken property

يحصل أو يعيّن رمز إلغاء يُستخدم لإلغاء عملية الاستخراج.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## ملاحظات

هذه الخاصية موجودة لإطار عمل .NET الإصدار 4.0 وما فوق.

## أمثلة

إلغاء استخراج أرشيف ISO بعد فترة زمنية معينة.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new IsoArchive("big.iso", new IsoLoadOptions() { CancellationToken = cts.Token }))
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

الاستخدام مع `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new ArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = Archive("big.iso", loadOptions))
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

الإلغاء يؤدي غالبًا إلى عدم استخراج بعض البيانات.

### انظر أيضًا

* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


