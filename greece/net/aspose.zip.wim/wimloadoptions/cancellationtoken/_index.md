---
title: "WimLoadOptions.CancellationToken"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "WimLoadOptions ιδιότητα. Λαμβάνει ή ορίζει ένα token ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής."
type: docs
weight: 20
url: /el/net/aspose.zip.wim/wimloadoptions/cancellationtoken/
---
## WimLoadOptions.CancellationToken property

Λαμβάνει ή ορίζει ένα token ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Παρατηρήσεις

Αυτή η ιδιότητα υπάρχει για το .NET Framework 4.0 και νεότερα.

## Παραδείγματα

Ακύρωση εξαγωγής αρχείου WIM μετά από κάποιο χρονικό διάστημα.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new WimArchive("big.wim", new WimLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
            a.Images[0].AllEntries.OfType<WimFileEntry>().First().Extract("data.bin");
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
    var loadOptions = new WimLoadOptions() { CancellationToken = cts.Token };
    using (var a = WimArchive("big.wim", loadOptions))
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

* class [WimLoadOptions](../)
* namespace [Aspose.Zip.Wim](../../wimloadoptions/)
* assembly [Aspose.Zip](../../../)


