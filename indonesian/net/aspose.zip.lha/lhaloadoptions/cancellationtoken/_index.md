---
title: "LhaLoadOptions.CancellationToken"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti LhaLoadOptions. Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi"
type: docs
weight: 20
url: /id/net/aspose.zip.lha/lhaloadoptions/cancellationtoken/
---
## LhaLoadOptions.CancellationToken property

Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Catatan

Properti ini ada untuk .NET Framework 4.0 ke atas.

## Contoh

Batalkan ekstraksi arsip LHA setelah waktu tertentu.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new LhaArchive("big.lha", new LhaLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new LhaLoadOptions() { CancellationToken = cts.Token };
    using (var a = new LhaArchive("big.arj", loadOptions))
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

* class [LhaLoadOptions](../)
* namespace [Aspose.Zip.Lha](../../lhaloadoptions/)
* assembly [Aspose.Zip](../../../)


