---
title: "LzxLoadOptions.CancellationToken"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "LzxLoadOptions properti. Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi"
type: docs
weight: 20
url: /id/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Catatan

Properti ini ada untuk .NET Framework 4.0 ke atas.

## Contoh

Batalkan ekstraksi arsip Lzx setelah waktu tertentu.

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

Menggunakan dengan `Task`

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

Pembatalan biasanya menghasilkan sebagian data tidak diekstrak.

### Lihat Juga

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


