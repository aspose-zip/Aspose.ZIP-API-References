---
title: "AlzArchiveLoadOptions.CancellationToken"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство AlzArchiveLoadOptions. Получает или задает токен отмены, используемый для прерывания операции извлечения."
type: docs
weight: 20
url: /ru/net/aspose.zip.alz/alzarchiveloadoptions/cancellationtoken/
---
## AlzArchiveLoadOptions.CancellationToken property

Получает или задает токен отмены, используемый для отмены операции извлечения.

```csharp
public CancellationToken CancellationToken { get; set; }
```

## Примечания

Это свойство существует для .NET Framework 4.0 и выше.

## Примеры

Отменить извлечение архива ALZ через определённое время.

```csharp
using (CancellationTokenSource cts = new CancellationTokenSource())
{
    cts.CancelAfter(TimeSpan.FromSeconds(60));
    using (var archive = new AlzArchive("big.alz", new AlzArchiveLoadOptions() { CancellationToken = cts.Token }))
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

* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


