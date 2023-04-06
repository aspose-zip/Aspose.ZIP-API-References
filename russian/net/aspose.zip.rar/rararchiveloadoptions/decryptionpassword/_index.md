---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP для справочника API .NET
description: RarArchiveLoadOptions свойство. Получает или задает пароль для расшифровки записей и имен записей.
type: docs
weight: 20
url: /ru/net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Получает или задает пароль для расшифровки записей и имен записей.

```csharp
public string DecryptionPassword { get; set; }
```

### Примеры

Вы можете указать пароль для расшифровки один раз при распаковке архива.

```csharp
using (FileStream fs = File.OpenRead("encrypted_archive.rar"))
{
    using (var extracted = File.Create("extracted.bin"))
    {
        using (RarArchive archive = new RarArchive(fs, new ArchiveLoadOptions() { DecryptionPassword = "p@s$" }))
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

### Смотрите также

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* пространство имен [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* сборка [Aspose.Zip](../../../)


