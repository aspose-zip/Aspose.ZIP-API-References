---
title: "Bzip2CompressionSettings.Bzip2CompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Bzip2CompressionSettings コンストラクタ。Bzip2CompressionSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/bzip2compressionsettings/bzip2compressionsettings/
---
## Bzip2CompressionSettings(int) {#constructor_1}

`[`Bzip2CompressionSettings`](../)` クラスの新しいインスタンスを初期化します。

```csharp
public Bzip2CompressionSettings(int blockSize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | Int32 | ブロックサイズ（百キロバイト単位）。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | ブロックサイズが1から9の範囲にありません。 |

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings(1))))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2CompressionSettings() {#constructor}

デフォルトのブロックサイズ（9百キロバイト）で、[`Bzip2CompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Bzip2CompressionSettings()
```

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new Bzip2CompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [Bzip2CompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../bzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


