---
title: "ArjLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство ArjLoadOptions. Получает или задаёт токен отмены, используемый для отмены операции извлечения"
type: docs
weight: 20
url: /ru/net/aspose.zip.arj/arjloadoptions/cancellationtoken/
---
## ArjLoadOptions.CancellationToken property

Получает или задает токен отмены, используемый для отмены операции извлечения.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Примечания

Это свойство существует для .NET Framework 4.0 и выше.

## Примеры

Отменить извлечение ARJ-архива после определённого времени.

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

Использование с `Task`

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

Отмена обычно приводит к тому, что часть данных не будет извлечена.

### См. также

* class [ArjLoadOptions](../)
* namespace [Aspose.Zip.Arj](../../arjloadoptions/)
* assembly [Aspose.Zip](../../../)


