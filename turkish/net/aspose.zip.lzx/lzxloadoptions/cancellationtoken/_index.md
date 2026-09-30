---
title: "LzxLoadOptions.CancellationToken"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LzxLoadOptions özelliği. Çıkarma işlemini iptal etmek için kullanılan bir iptal belirtecini alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

Çıkarma işlemini iptal etmek için kullanılan bir iptal belirtecini alır veya ayarlar.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Açıklamalar

Bu özellik .NET Framework 4.0 ve üzeri için mevcuttur.

## Örnekler

Belirli bir süreden sonra Lzx arşivi çıkarımını iptal edin.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new LzxArchive("big.lzx", new LzxLoadOptions() { CancellationToken = cts.Token }))
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

`Task` ile kullanım

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    LzxLoadOptions loadOptions = new LzxLoadOptions() { CancellationToken = cts.Token };
    using (LzxArchive a = new LzxArchive("big.lzx", loadOptions))
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

İptal, genellikle bazı verilerin çıkarılmamasına neden olur.

### Ayrıca Bakınız

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


