---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство AlzArchiveLoadOptions. Получает или задает пароль для расшифровки записей."
type: docs
weight: 30
url: /ru/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

Получает или задает пароль для расшифровки записей.

```csharp
public string DecryptionPassword { get; set; }
```

## Примеры

Вы можете указать пароль для расшифровки один раз при извлечении архива.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.alz"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (var archive = new AlzArchive(fs, new AlzArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


