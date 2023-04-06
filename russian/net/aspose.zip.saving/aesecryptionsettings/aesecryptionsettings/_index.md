---
title: AesEcryptionSettings.AesEcryptionSettings
second_title: Aspose.ZIP для справочника API .NET
description: AesEcryptionSettings строитель. Инициализирует новый экземплярAesEcryptionSettings класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Инициализирует новый экземпляр[`AesEcryptionSettings`](../) класс.

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования или дешифрования. |
| method | EncryptionMethod | Опция алгоритма, указывающая размер блока шифра. |

### Исключения

| исключение | условие |
| --- | --- |
| NotSupportedException | *method* не является одним изAES128 ,AES192 , илиAES256. |

### Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### Смотрите также

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../aesecryptionsettings/)
* сборка [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Инициализирует новый экземпляр[`AesEcryptionSettings`](../)класс без пароля.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| method | EncryptionMethod | Опция алгоритма, указывающая размер блока шифра. |

### Смотрите также

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../aesecryptionsettings/)
* сборка [Aspose.Zip](../../../)


