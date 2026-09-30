---
title: "TraditionalEncryptionSettings.TraditionalEncryptionSettings"
second_title: "Aspose.ZIP for .NET API Справочник"
description: "Конструктор TraditionalEncryptionSettings. Инициализирует новый экземпляр класса TraditionalEncryptionSettings"
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Инициализирует новый экземпляр класса [`TraditionalEncryptionSettings`](../).

```csharp
public TraditionalEncryptionSettings(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования. |

## Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### См. также

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Инициализирует новый экземпляр класса [`TraditionalEncryptionSettings`](../) с пользовательской кодировкой.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования. |
| кодировка | Кодировка | Кодировка символов пароля. |

## Примечания

Использование этого конструктора не рекомендуется. Установка кодировки может противоречить стандарту и привести к несовместимому архиву.

## Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### См. также

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Создаёт новый экземпляр класса [`TraditionalEncryptionSettings`](../) без пароля.

```csharp
public TraditionalEncryptionSettings()
```

### См. также

* class [TraditionalEncryptionSettings](../)
* namespace [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* assembly [Aspose.Zip](../../../)


