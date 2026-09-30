---
title: "ArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство ArchiveLoadOptions. Возвращает или задает пароль для расшифровки записей"
type: docs
weight: 30
url: /ru/net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

Получает или задает пароль для расшифровки записей.

```csharp
public string DecryptionPassword { get; set; }
```

## Примеры

Вы можете указать пароль для расшифровки один раз при извлечении архива.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.zip"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (var archive = new Archive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
        {
            using (var decompressed = archive.Entries[0].Open())
            {
                byte[] b = new byte[8192];
                int bytesRead;
                while (0 < (bytesRead = decompressed.Read(b, 0, b.Length)))
                    extracted.Write(b, 0, bytesRead);
                
            }
        }
    }
}
```

### См. также

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


