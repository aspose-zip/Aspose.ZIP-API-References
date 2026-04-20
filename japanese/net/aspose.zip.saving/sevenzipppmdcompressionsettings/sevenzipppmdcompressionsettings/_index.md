---
title: SevenZipPPMdCompressionSettings.SevenZipPPMdCompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: SevenZipPPMdCompressionSettings コンストラクタ. 7z アーカイブ内の PPMd 圧縮方法の設定をインスタンス化します
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/sevenzipppmdcompressionsettings/sevenzipppmdcompressionsettings/
---
## SevenZipPPMdCompressionSettings(byte, int) {#constructor_1}

7z アーカイブ内の PPMd 圧縮方法の設定をインスタンス化します。

```csharp
public SevenZipPPMdCompressionSettings(byte maxOrder, int suballocatorSize)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| maxOrder | Byte | 最大注文。 |
| suballocatorSize | Int32 | MB サブアロケータのメモリ サイズが消費される可能性があります。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | *maxOrder*が 2 から 32 の間でない、または*suballocatorSize*は 1 から 1024 の間ではありません。 |

### 備考

モデルオーダーが大きいほど、ほぼ確実に圧縮率が向上し、メモリと CPU の使用量が確実に増加します。

PPMd アルゴリズムは、特に大きなファイルで使用したり、大きなモデル順序で使用したりする場合に、大量のメモリを必要とする場合があります。

### 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings(4, 32))))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 関連項目

* class [SevenZipPPMdCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## SevenZipPPMdCompressionSettings() {#constructor}

7z アーカイブ内の PPMd 圧縮方法の設定を、デフォルトのモデル順序とサブアロケーター サイズでインスタンス化します。

```csharp
public SevenZipPPMdCompressionSettings()
```

### 備考

デフォルトのモデル順序は 6 で、サブアロケータのサイズは 16MB です。

### 例

```csharp
using (SevenZipArchive archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipPPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                        
    archive.Save(sevenZipFile);
 }
```

### 関連項目

* class [SevenZipPPMdCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../sevenzipppmdcompressionsettings/)
* 組み立て [Aspose.Zip](../../../)


