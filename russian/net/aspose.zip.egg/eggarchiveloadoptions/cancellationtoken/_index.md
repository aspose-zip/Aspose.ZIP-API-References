---
title: "EggArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство EggArchiveLoadOptions. Получает или задаёт токен отмены, используемый для прерывания операции извлечения."
type: docs
weight: 20
url: /ru/net/aspose.zip.egg/eggarchiveloadoptions/cancellationtoken/
---
## EggArchiveLoadOptions.CancellationToken property

Получает или задает токен отмены, используемый для отмены операции извлечения.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Примечания

Это свойство существует для .NET Framework 4.0 и выше.

## Примеры

Отменить извлечение архива EGG после определённого времени.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (var archive = new EggArchive("big.egg", new EggArchiveLoadOptions() { CancellationToken = cts.Token }))
    {
        try
        {
            archive.Entries[0].Extract("data.bin");
        }
        catch(OperationCanceledException)
        {
            Console.WriteLine("Extraction was cancelled after 60 seconds");
        }
    }
}
```

### См. также

* class [EggArchiveLoadOptions](../)
* namespace [Aspose.Zip.Egg](../../eggarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


