---
title: "SevenZipLoadOptions.CancellationToken"
second_title: "Aspose.ZIP için .NET API Referansı"
description: "SevenZipLoadOptions özelliği. Çıkarma işlemini iptal etmek için kullanılan bir iptal belirtecini alır veya ayarlar"
type: docs
weight: 20
url: /tr/net/aspose.zip.sevenzip/sevenziploadoptions/cancellationtoken/
---
## SevenZipLoadOptions.CancellationToken property

Çıkarma işlemini iptal etmek için kullanılan bir iptal belirtecini alır veya ayarlar.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Açıklamalar

Bu özellik .NET Framework 4.0 ve üzeri için mevcuttur.

## Örnekler

Belirli bir süreden sonra 7Z arşiv çıkarma işlemini iptal edin.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new SevenZipArchive("big.7z", new SevenZipLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new SevenZipLoadOptions() { CancellationToken = cts.Token };
    using (var a = new SevenZipArchive("big.7z", loadOptions))
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

* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


