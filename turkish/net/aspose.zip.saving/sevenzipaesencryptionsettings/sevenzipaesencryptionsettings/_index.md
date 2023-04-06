---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: SevenZipAESEncryptionSettings inşaatçı. Yeni bir örneğini başlatır.SevenZipAESEncryptionSettings sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Yeni bir örneğini başlatır.[`SevenZipAESEncryptionSettings`](../) sınıf.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| password | String | Şifreleme veya şifre çözme için parola. |

### Örnekler

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Ayrıca bakınız

* class [SevenZipAESEncryptionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* toplantı [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Yeni bir örneğini başlatır.[`SevenZipAESEncryptionSettings`](../) harici cipher. ile sınıf

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| cipher | SevenZipCipher | Özel AES uygulaması. |

### Örnekler

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Ayrıca bakınız

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* toplantı [Aspose.Zip](../../../)


