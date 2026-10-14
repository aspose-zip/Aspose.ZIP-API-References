---
title: "PPMdCompressionSettings.PPMdCompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "PPMdCompressionSettings コンストラクタ。PPMdCompressionSettings クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

[`PPMdCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| modelOrder | Int32 | モデルの順序。 |
| suballocatorSize | Int32 | サブアロケータが消費する可能性のあるメモリサイズ（MB）。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder* は 2 から 16 の間ではありません。 - または - *suballocatorSize* は 1 から 256 の間ではありません。 |

## 備考

モデルオーダーが大きくなるほど、ほぼ確実に圧縮率は向上しますが、メモリと CPU 使用量も確実に増加します。

PPMd アルゴリズムは大量のメモリを必要とする可能性があり、特に大きなファイルや大きなモデルオーダーで使用する場合に顕著です。ppmd が与えられたメモリより多く必要とすると、圧縮率が低下します。

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

デフォルトのモデル順序とサブアロケータサイズを使用して、[`PPMdCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public PPMdCompressionSettings()
```

## 備考

デフォルトのモデル順序は 8 で、サブアロケータサイズは 50MB です。

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [PPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


