---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Свойство SevenZipLoadOptions. Получает или задаёт пароль для расшифровки записей и имён записей"
type: docs
weight: 30
url: /ru/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

Получает или задает пароль для дешифрования записей и имен записей.

```csharp
public string DecryptionPassword { get; set; }
```

## Примеры

Вы можете указать пароль для расшифровки один раз при извлечении архива.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.7z"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (SevenZipArchive archive = new SevenZipArchive(fs, new SevenZipLoadOptions() { DecryptionPassword = "p@s$" }))
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

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


