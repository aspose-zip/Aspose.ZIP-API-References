---
title: "Класс SevenZipEncryptionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Класс Aspose.Zip.Saving.SevenZipEncryptionSettings. Базовый класс для настроек нескольких методов шифрования 7z"
type: docs
weight: 1060
url: /ru/net/aspose.zip.saving/sevenzipencryptionsettings/
---
## SevenZipEncryptionSettings class

Базовый класс настроек для нескольких методов шифрования 7z.

```csharp
public abstract class SevenZipEncryptionSettings
```

## Свойства

| Имя | Описание |
| --- | --- |
| [EncryptHeader](../../aspose.zip.saving/sevenzipencryptionsettings/encryptheader/) { get; set; } | Получает или задает значение, указывающее на шифрование заголовка. |
| [Password](../../aspose.zip.saving/sevenzipencryptionsettings/password/) { get; set; } | Получает или задает пароль для шифрования или дешифрования. |

## Примечания

AES‑256 — единственный возможный метод шифрования для 7z‑архива. Поэтому [`SevenZipAESEncryptionSettings`](../sevenzipaesencryptionsettings/) является единственной реализацией.

### См. также

* namespace [Aspose.Zip.Saving](../../aspose.zip.saving/)
* assembly [Aspose.Zip](../../)


