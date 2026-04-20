---
title: Bzip2CompressionSettings.Bzip2CompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: Bzip2CompressionSettings コンストラクタ. の新しいインスタンスを初期化しますBzip2CompressionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

の新しいインスタンスを初期化します[`Bzip2CompressionSettings`](../)class.

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| blockSize | Int32 | 数百キロバイト単位のブロック サイズ。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | ブロック サイズが 1 から 9 の間ではありません。 |

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [Bzip2CompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

の新しいインスタンスを初期化します[`Bzip2CompressionSettings`](../)デフォルトのブロック サイズを持つクラスで、900 キロバイトに相当します。

```csharp
public Bzip2CompressionSettings()
```

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [Bzip2CompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* 組み立て [Aspose.Zip](../../../)


