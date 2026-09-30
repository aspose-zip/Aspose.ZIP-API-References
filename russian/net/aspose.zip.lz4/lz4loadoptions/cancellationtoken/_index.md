---
title: "Lz4LoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство Lz4LoadOptions. Получает или задаёт токен отмены, используемый для отмены операции извлечения."
type: docs
weight: 20
url: /ru/net/aspose.zip.lz4/lz4loadoptions/cancellationtoken/
---
## Lz4LoadOptions.CancellationToken property

Получает или задает токен отмены, используемый для отмены операции извлечения.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Примечания

Это свойство существует для .NET Framework 4.0 и выше.

## Примеры

Отменить извлечение lz4-архива после определённого времени.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60)); 
    using (var a = new Lz4Archive("big.lz4", new Lz4LoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
             a.Extract("data.bin");
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
    var loadOptions = new Lz4LoadOptions() { CancellationToken = cts.Token };
    using (var a = Lz4Archive("big.lz4", loadOptions))
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

* class [Lz4LoadOptions](../)
* namespace [Aspose.Zip.Lz4](../../lz4loadoptions/)
* assembly [Aspose.Zip](../../../)


