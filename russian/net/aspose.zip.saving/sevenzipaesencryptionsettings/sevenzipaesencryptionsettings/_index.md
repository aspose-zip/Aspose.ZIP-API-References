---
title: SevenZipAESEncryptionSettings.SevenZipAESEncryptionSettings
second_title: Aspose.ZIP для справочника API .NET
description: SevenZipAESEncryptionSettings строитель. Инициализирует новый экземплярSevenZipAESEncryptionSettings класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/sevenzipaesencryptionsettings/sevenzipaesencryptionsettings/
---
## SevenZipAESEncryptionSettings(string) {#constructor_1}

Инициализирует новый экземпляр[`SevenZipAESEncryptionSettings`](../) класс.

```csharp
public SevenZipAESEncryptionSettings(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования или дешифрования. |

### Примеры

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings("p@s$"))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Смотрите также

* class [SevenZipAESEncryptionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* сборка [Aspose.Zip](../../../)

---

## SevenZipAESEncryptionSettings(SevenZipCipher) {#constructor}

Инициализирует новый экземпляр[`SevenZipAESEncryptionSettings`](../) класс с внешним шифром.

```csharp
public SevenZipAESEncryptionSettings(SevenZipCipher cipher)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| cipher | SevenZipCipher | Пользовательская реализация AES. |

### Примеры

```csharp
SevenZipCipher cipher = ComposeMyCipher();
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(null, new SevenZipAESEncryptionSettings(cipher))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.7z");
}
```

### Смотрите также

* class [SevenZipCipher](../../../aspose.zip.crypto/sevenzipcipher/)
* class [SevenZipAESEncryptionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../sevenzipaesencryptionsettings/)
* сборка [Aspose.Zip](../../../)


