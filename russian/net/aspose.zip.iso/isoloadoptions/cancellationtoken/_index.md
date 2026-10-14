---
title: "IsoLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство IsoLoadOptions. Получает или задает токен отмены, используемый для прерывания операции извлечения"
type: docs
weight: 20
url: /ru/net/aspose.zip.iso/isoloadoptions/cancellationtoken/
---
## IsoLoadOptions.CancellationToken property

Получает или задает токен отмены, используемый для отмены операции извлечения.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Примечания

Это свойство существует для .NET Framework 4.0 и выше.

## Примеры

Отменить извлечение ISO-архива после определённого времени.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new IsoArchive("big.iso", new IsoLoadOptions() { CancellationToken = cts.Token }))
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

Использование с `Task`

```csharp
CancellationTokenSource cts = new CancellationTokenSource();
cts.CancelAfter(TimeSpan.FromSeconds(60));
Task t = Task.Run(delegate()
{
    var loadOptions = new ArchiveLoadOptions() { CancellationToken = cts.Token };
    using (var a = Archive("big.iso", loadOptions))
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

Отмена обычно приводит к тому, что часть данных не будет извлечена.

### См. также

* class [IsoLoadOptions](../)
* namespace [Aspose.Zip.Iso](../../isoloadoptions/)
* assembly [Aspose.Zip](../../../)


