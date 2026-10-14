---
title: "LzipLoadOptions.CancellationToken"
second_title: "مرجع API لـ Aspose.ZIP لـ .NET"
description: "خاصية LzipLoadOptions. تحصل أو تعيين رمز إلغاء يُستخدم لإلغاء عملية الاستخراج."
type: docs
weight: 20
url: /ar/net/aspose.zip.lzip/lziploadoptions/cancellationtoken/
---
## LzipLoadOptions.CancellationToken property

يحصل أو يعيّن رمز إلغاء يُستخدم لإلغاء عملية الاستخراج.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## ملاحظات

هذه الخاصية موجودة لإطار عمل .NET الإصدار 4.0 وما فوق.

## أمثلة

إلغاء استخراج أرشيف lzip بعد مدة معينة.

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

الاستخدام مع `Task`

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

الإلغاء يؤدي غالبًا إلى عدم استخراج بعض البيانات.

### انظر أيضًا

* class [LzipLoadOptions](../)
* namespace [Aspose.Zip.Lzip](../../lziploadoptions/)
* assembly [Aspose.Zip](../../../)


