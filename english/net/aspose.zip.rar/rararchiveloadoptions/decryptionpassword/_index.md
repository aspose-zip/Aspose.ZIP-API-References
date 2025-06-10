---
title: RarArchiveLoadOptions.DecryptionPassword
second_title: Aspose.ZIP for .NET API Reference
description: RarArchiveLoadOptions property. Gets or sets the password to decrypt entries and entry names
type: docs
weight: 30
url: /net/aspose.zip.rar/rararchiveloadoptions/decryptionpassword/
---
## RarArchiveLoadOptions.DecryptionPassword property

Gets or sets the password to decrypt entries and entry names.

```csharp
public string DecryptionPassword { get; set; }
```

## Examples

You can provide decryption password once on archive extraction.

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

### See Also

* method [Open](../../rararchiveentry/open/)
* class [RarArchiveLoadOptions](../)
* namespace [Aspose.Zip.Rar](../../rararchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


