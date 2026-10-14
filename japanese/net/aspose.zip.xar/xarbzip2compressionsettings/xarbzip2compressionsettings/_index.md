---
title: "XarBzip2CompressionSettings.XarBzip2CompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "XarBzip2CompressionSettings コンストラクタ。XarBzip2CompressionSettings クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.xar/xarbzip2compressionsettings/xarbzip2compressionsettings/
---
## XarBzip2CompressionSettings(int) {#constructor_1}

[`XarBzip2CompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public XarBzip2CompressionSettings(int blockSize)
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
using (XarArchive archive = new XarArchive())
{
    archive.CreateEntry("data.bin", "data.bin", new XarBzip2CompressionSettings(1));
    archive.Save("archive.xar");
}
```

### 関連項目

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## XarBzip2CompressionSettings() {#constructor}

[`XarBzip2CompressionSettings`](../) クラスの新しいインスタンスを初期化します（デフォルトのブロックサイズは 9 百キロバイトに相当します）。

```csharp
public XarBzip2CompressionSettings()
```

### 関連項目

* class [XarBzip2CompressionSettings](../)
* namespace [Aspose.Zip.Xar](../../xarbzip2compressionsettings/)
* assembly [Aspose.Zip](../../../)


