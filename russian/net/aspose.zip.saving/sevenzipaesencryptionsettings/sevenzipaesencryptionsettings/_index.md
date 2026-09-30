---
title: "SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор SevenZipAESEncryptionSettings. Инициализирует новый экземпляр класса SevenZipAESEncryptionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Инициализирует новый экземпляр класса [`SevenZipAESEncryptionSettings`](../).

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования или дешифрования. |

## Примеры

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### См. также

* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Инициализирует новый экземпляр класса [`SevenZipAESEncryptionSettings`](../) с внешним шифром.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| шифр | SevenZipCipher | Пользовательская реализация AES. |

## Примеры

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### См. также

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* assembly [Aspose.Zip](../../../)


