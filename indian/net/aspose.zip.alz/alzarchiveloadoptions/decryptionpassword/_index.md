---
title: "AlzArchiveLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "AlzArchiveLoadOptions प्रॉपर्टी। एंट्रीज़ को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त या सेट करती है।"
type: docs
weight: 30
url: /hi/net/aspose.zip.alz/alzarchiveloadoptions/decryptionpassword/
---
## AlzArchiveLoadOptions.DecryptionPassword property

एंट्रीज़ को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है या सेट करता है।

```csharp
public string DecryptionPassword { get; set; }
```

## उदाहरण

आप आर्काइव निष्कर्षण पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

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

### संबंधित देखें

* method [Open](../../alzentry/open/)
* class [AlzArchiveLoadOptions](../)
* namespace [Aspose.Zip.Alz](../../alzarchiveloadoptions/)
* assembly [Aspose.Zip](../../../)


