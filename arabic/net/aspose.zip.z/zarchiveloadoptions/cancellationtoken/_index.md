---
title: "ZArchiveLoadOptions.CancellationToken"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية ZArchiveLoadOptions. تحصل أو تعيين رمز إلغاء يُستخدم لإلغاء عملية الاستخراج"
type: docs
weight: 20
url: /ar/net/aspose.zip.z/zarchiveloadoptions/cancellationtoken/
---
## ZArchiveLoadOptions.CancellationToken property

يحصل أو يعيّن رمز إلغاء يُستخدم لإلغاء عملية الاستخراج.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## ملاحظات

هذه الخاصية موجودة لإطار عمل .NET الإصدار 4.0 وما فوق.

## أمثلة

إلغاء استخراج أرشيف Z بعد فترة زمنية معينة.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new ZArchive("big.z", new ZArchiveLoadOptions() { CancellationToken = cts.Token }))
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

الاستخدام مع `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new ZArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = ZArchive("big.z", loadOptions))
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

* class [ZArchiveLoadOptions](../)
* namespace [Aspose.Zip.Z](../../zarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


