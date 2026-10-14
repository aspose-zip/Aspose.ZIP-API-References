---
title: "LzipLoadOptions.CancellationToken"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "LzipLoadOptions özelliği. Çıkarma işlemini iptal etmek için kullanılan bir iptal belirtecini alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.zip.lzip/lziploadoptions/cancellationtoken/
---
## LzipLoadOptions.CancellationToken property

Çıkarma işlemini iptal etmek için kullanılan bir iptal belirtecini alır veya ayarlar.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Açıklamalar

Bu özellik .NET Framework 4.0 ve üzeri için mevcuttur.

## Örnekler

Belirli bir süreden sonra lzip arşivi çıkarımını iptal et.

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

`Task` ile kullanım

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

İptal, genellikle bazı verilerin çıkarılmamasına neden olur.

### Ayrıca Bakınız

* class [LzipLoadOptions](../)
* namespace [Aspose.Zip.Lzip](../../lziploadoptions/)
* assembly [Aspose.Zip](../../../)


