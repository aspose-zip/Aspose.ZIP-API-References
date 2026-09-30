---
title: "LzxLoadOptions.CancellationToken"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "LzxLoadOptions ιδιότητα. Λαμβάνει ή ορίζει ένα διακριτικό ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής."
type: docs
weight: 20
url: /el/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

Λαμβάνει ή ορίζει ένα token ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Παρατηρήσεις

Αυτή η ιδιότητα υπάρχει για το .NET Framework 4.0 και νεότερα.

## Παραδείγματα

Ακυρώστε την εξαγωγή του αρχείου Lzx μετά από κάποιο χρονικό διάστημα.

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

Χρήση με `Task`

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

Η ακύρωση συνήθως οδηγεί στο ότι κάποια δεδομένα δεν εξάγονται.

### Δείτε επίσης

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


