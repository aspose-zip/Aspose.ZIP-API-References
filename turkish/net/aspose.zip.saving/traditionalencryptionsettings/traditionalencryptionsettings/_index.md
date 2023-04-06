---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP for .NET API Referansı
description: TraditionalEncryptionSettings inşaatçı. Yeni bir örneğini başlatır.TraditionalEncryptionSettings sınıf.
type: docs
weight: 10
url: /tr/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Yeni bir örneğini başlatır.[`TraditionalEncryptionSettings`](../) sınıf.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| password | String | Şifreleme için şifre. |

### Örnekler

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [TraditionalEncryptionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* toplantı [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Yeni bir örneğini başlatır.[`TraditionalEncryptionSettings`](../) kullanıcı tanımlı kodlamaya sahip sınıf.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Parametre | Tip | Tanım |
| --- | --- | --- |
| password | String | Şifreleme için şifre. |
| encoding | Encoding | Parola karakterleri için kodlama. |

### Notlar

Bu yapıcının kullanılması önerilmez. Kodlamanın ayarlanması standartla çelişebilir ve uyumsuz arşiv oluşturabilir.

### Örnekler

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Ayrıca bakınız

* class [TraditionalEncryptionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* toplantı [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Yeni bir örneğini başlatır.[`TraditionalEncryptionSettings`](../)şifresiz sınıf.

```csharp
public TraditionalEncryptionSettings()
```

### Ayrıca bakınız

* class [TraditionalEncryptionSettings](../)
* ad alanı [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* toplantı [Aspose.Zip](../../../)


