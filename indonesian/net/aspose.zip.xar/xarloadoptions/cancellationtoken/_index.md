---
title: "XarLoadOptions.CancellationToken"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti XarLoadOptions. Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi."
type: docs
weight: 20
url: /id/net/aspose.zip.xar/xarloadoptions/cancellationtoken/
---
## XarLoadOptions.CancellationToken property

Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Catatan

Properti ini ada untuk .NET Framework 4.0 ke atas.

## Contoh

Batalkan ekstraksi arsip XAR setelah waktu tertentu.

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

Menggunakan dengan `Task`

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

Pembatalan biasanya menghasilkan sebagian data tidak diekstrak.

### Lihat Juga

* class [XarLoadOptions](../)
* namespace [Aspose.Zip.Xar](../../xarloadoptions/)
* assembly [Aspose.Zip](../../../)


