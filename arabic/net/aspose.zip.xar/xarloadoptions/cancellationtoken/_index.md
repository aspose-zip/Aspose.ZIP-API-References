---
title: "XarLoadOptions.CancellationToken"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية XarLoadOptions. تحصل أو تعيين رمز إلغاء يُستخدم لإلغاء عملية الاستخراج."
type: docs
weight: 20
url: /ar/net/aspose.zip.xar/xarloadoptions/cancellationtoken/
---
## XarLoadOptions.CancellationToken property

يحصل أو يعيّن رمز إلغاء يُستخدم لإلغاء عملية الاستخراج.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## ملاحظات

هذه الخاصية موجودة لإطار عمل .NET الإصدار 4.0 وما فوق.

## أمثلة

إلغاء استخراج أرشيف XAR بعد مدة معينة.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new XarArchive("big.xar", new XarLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             (XarFileEntry)(a.Entries.First()).Extract("data.bin");
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
    var loadOptions = new XarLoadOptions() { CancellationToken = cts.Token };
    using (var a = new XarArchive("big.xar", loadOptions))
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

* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


