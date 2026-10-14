---
title: "SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipPPMdCompressionSettings コンストラクタ。7z アーカイブ内の PPMd 圧縮メソッド用設定をインスタンス化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

7z アーカイブ内の PPMd 圧縮方式の設定をインスタンス化します。

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| maxOrder | Byte | 最大オーダー。 |
| suballocatorSize | Int32 | サブアロケータが消費する可能性のあるメモリサイズ（MB）。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder* は 2 から 32 の間ではなく、または *suballocatorSize* は 1 から 1024 の間ではありません。 |

## 備考

モデルオーダーが大きくなるほど、ほぼ確実に圧縮率は向上しますが、メモリと CPU 使用量も確実に増加します。

PPMd アルゴリズムは大量のメモリを必要とする可能性があり、特に大きなファイルや大きなモデルオーダーで使用する場合に顕著です。ppmd が与えられたメモリより多く必要とすると、圧縮率が低下します。

## 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 関連項目

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

デフォルトのモデル順序とサブアロケータサイズで、7z アーカイブ内の PPMd 圧縮方式の設定をインスタンス化します。

```csharp
public SevenZipPPMdCompressionSettings()
```

## 備考

デフォルトのモデルオーダーは 6 で、サブアロケータサイズは 16MB です。

## 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 関連項目

* class [SevenZipPPMdCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* assembly [Aspose.Zip](../../../)


