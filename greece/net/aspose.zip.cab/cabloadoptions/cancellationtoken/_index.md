---
title: "CabLoadOptions.CancellationToken"
second_title: "Aspose.ZIP για .NET API Αναφορά"
description: "Ιδιότητα CabLoadOptions. Επιστρέφει ή ορίζει ένα token ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής"
type: docs
weight: 20
url: /el/net/aspose.zip.cab/cabloadoptions/cancellationtoken/
---
## CabLoadOptions.CancellationToken property

Λαμβάνει ή ορίζει ένα token ακύρωσης που χρησιμοποιείται για την ακύρωση της λειτουργίας εξαγωγής.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Παρατηρήσεις

Αυτή η ιδιότητα υπάρχει για το .NET Framework 4.0 και νεότερα.

## Παραδείγματα

Ακυρώστε την εξαγωγή του αρχείου CAB μετά από κάποιο χρονικό διάστημα.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new CabArchive("big.cab", new CabLoadOptions() { CancellationToken = cts.Token }))
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
    var loadOptions = new CabLoadOptions() { CancellationToken = cts.Token };
    using (var a = new CabArchive("big.cab", loadOptions))
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

* class [CabLoadOptions](../)
* namespace [Aspose.Zip.Cab](../../cabloadoptions/)
* assembly [Aspose.Zip](../../../)


