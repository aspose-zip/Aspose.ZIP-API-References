---
title: "LzxLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство LzxLoadOptions. Получает или задает токен отмены, используемый для отмены операции извлечения"
type: docs
weight: 20
url: /ru/net/aspose.zip.lzx/lzxloadoptions/cancellationtoken/
---
## LzxLoadOptions.CancellationToken property

Получает или задает токен отмены, используемый для отмены операции извлечения.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Примечания

Это свойство существует для .NET Framework 4.0 и выше.

## Примеры

Отменить извлечение архива Lzx после определённого времени.

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

Использование с `Task`

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

Отмена обычно приводит к тому, что часть данных не будет извлечена.

### См. также

* class [LzxLoadOptions](../)
* namespace [Aspose.Zip.Lzx](../../lzxloadoptions/)
* assembly [Aspose.Zip](../../../)


