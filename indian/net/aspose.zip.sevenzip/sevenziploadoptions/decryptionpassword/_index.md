---
title: "SevenZipLoadOptions.DecryptionPassword"
second_title: "Aspose.ZIP के लिए .NET API संदर्भ"
description: "SevenZipLoadOptions प्रॉपर्टी। प्रविष्टियों और प्रविष्टि नामों को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है या सेट करता है"
type: docs
weight: 30
url: /hi/net/aspose.zip.sevenzip/sevenziploadoptions/decryptionpassword/
---
## SevenZipLoadOptions.DecryptionPassword property

एंट्रीज़ और एंट्री नामों को डिक्रिप्ट करने के लिए पासवर्ड प्राप्त करता है या सेट करता है।

```csharp
public string DecryptionPassword { get; set; }
```

## उदाहरण

आप आर्काइव निष्कर्षण पर एक बार डिक्रिप्शन पासवर्ड प्रदान कर सकते हैं।

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

### संबंधित देखें

* method [Open](../../sevenziparchiveentry/open/)
* class [SevenZipLoadOptions](../)
* namespace [Aspose.Zip.SevenZip](../../sevenziploadoptions/)
* assembly [Aspose.Zip](../../../)


