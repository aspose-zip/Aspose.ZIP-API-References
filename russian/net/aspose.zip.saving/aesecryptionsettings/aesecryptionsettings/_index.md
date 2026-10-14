---
title: "AesEcryptionSettings.AesEcryptionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор AesEcryptionSettings. Инициализирует новый экземпляр класса AesEcryptionSettings."
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/aesecryptionsettings/aesecryptionsettings/
---
## AesEcryptionSettings(string, EncryptionMethod) {#constructor_1}

Инициализирует новый экземпляр класса [`AesEcryptionSettings`](../).

```csharp
public AesEcryptionSettings(string password, EncryptionMethod method)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования или дешифрования. |
| метод | EncryptionMethod | Параметр алгоритма, указывающий размер блока шифра. |

### Исключения

| исключение | условие |
| --- | --- |
| NotSupportedException | *method* не является одним из AES128, AES192 или AES256. |

## Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new AesEcryptionSettings("p@s$", EncryptionMethod.AES256))))
{
   archive.CreateEntry("data.bin", "data.bin");
   archive.Save("archive.zip");
}
```

### См. также

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## AesEcryptionSettings(EncryptionMethod) {#constructor}

Инициализирует новый экземпляр класса [`AesEcryptionSettings`](../) без пароля.

```csharp
public AesEcryptionSettings(EncryptionMethod method)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| метод | EncryptionMethod | Параметр алгоритма, указывающий размер блока шифра. |

### Исключения

| исключение | условие |
| --- | --- |
| NotSupportedException | *method* не является одним из AES128, AES192 или AES256. |

### См. также

* enum [EncryptionMethod](../../encryptionmethod/)
* class [AesEcryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../aesecryptionsettings/)
* assembly [Aspose.Zip](../../../)


