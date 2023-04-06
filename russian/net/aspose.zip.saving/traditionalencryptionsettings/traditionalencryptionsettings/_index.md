---
title: TraditionalEncryptionSettings.TraditionalEncryptionSettings
second_title: Aspose.ZIP для справочника API .NET
description: TraditionalEncryptionSettings строитель. Инициализирует новый экземплярTraditionalEncryptionSettings класс.
type: docs
weight: 10
url: /ru/net/aspose.zip.saving/traditionalencryptionsettings/traditionalencryptionsettings/
---
## TraditionalEncryptionSettings(string) {#constructor_1}

Инициализирует новый экземпляр[`TraditionalEncryptionSettings`](../) класс.

```csharp
public TraditionalEncryptionSettings(string password)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования. |

### Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p@s$"))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Смотрите также

* class [TraditionalEncryptionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* сборка [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings(string, Encoding) {#constructor_2}

Инициализирует новый экземпляр[`TraditionalEncryptionSettings`](../) класс с пользовательской кодировкой.

```csharp
public TraditionalEncryptionSettings(string password, Encoding encoding)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| password | String | Пароль для шифрования. |
| encoding | Encoding | Кодировка символов пароля. |

### Примечания

Использование этого конструктора не рекомендуется. Установка кодировки может противоречить стандарту и создавать несовместимый архив.

### Примеры

```csharp
using (var archive = new Archive(new ArchiveEntrySettings(null, new TraditionalEncryptionSettings("p£s$", System.Text.Encoding.ASCII))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### Смотрите также

* class [TraditionalEncryptionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* сборка [Aspose.Zip](../../../)

---

## TraditionalEncryptionSettings() {#constructor}

Инициализирует новый экземпляр[`TraditionalEncryptionSettings`](../)класс без пароля.

```csharp
public TraditionalEncryptionSettings()
```

### Смотрите также

* class [TraditionalEncryptionSettings](../)
* пространство имен [Aspose.Zip.Saving](../../traditionalencryptionsettings/)
* сборка [Aspose.Zip](../../../)


