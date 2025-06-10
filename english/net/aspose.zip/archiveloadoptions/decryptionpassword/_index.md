---
title: ArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP for .NET API Reference
description: ArchiveLoadOptions property. Gets or sets the password to decrypt entries
type: docs
weight: 30
url: /net/aspose.zip/archiveloadoptions/decryptionpassword/
---
## ArchiveLoadOptions.DecryptionPassword property

Gets or sets the password to decrypt entries.

```csharp
public string DecryptionPassword { get; set; }
```

## Examples

You can provide decryption password once on archive extraction.

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

### See Also

* method [Open](../../archiveentry/open/)
* class [ArchiveLoadOptions](../)
* namespace [Aspose.Zip](../../archiveloadoptions/)
* assembly [Aspose.Zip](../../../)


