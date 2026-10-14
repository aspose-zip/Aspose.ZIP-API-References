---
title: "ArjLoadOptions.CancellationToken"
second_title: "Aspose.ZIP untuk Referensi API .NET"
description: "Properti ArjLoadOptions. Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi."
type: docs
weight: 20
url: /id/net/aspose.zip.arj/arjloadoptions/cancellationtoken/
---
## ArjLoadOptions.CancellationToken property

Mendapatkan atau mengatur token pembatalan yang digunakan untuk membatalkan operasi ekstraksi.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Catatan

Properti ini ada untuk .NET Framework 4.0 ke atas.

## Contoh

Batalkan ekstraksi arsip ARJ setelah waktu tertentu.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new ArjArchive("big.arj", new ArjLoadOptions() { CancellationToken = cts.Token }))
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
    ArjLoadOptions loadOptions = new ArjLoadOptions() { CancellationToken = cts.Token };
    using (ArjArchive a = new ArjArchive("big.arj", loadOptions))
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

* class [ArjLoadOptions](../)
* namespace [Aspose.Zip.Arj](../../arjloadoptions/)
* assembly [Aspose.Zip](../../../)


