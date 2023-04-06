---
title: PPMdCompressionSettings.PPMdCompressionSettings
second_title: Aspose.ZIP for .NET API リファレンス
description: PPMdCompressionSettings コンストラクタ. の新しいインスタンスを初期化しますPPMdCompressionSettingsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/ppmdcompressionsettings/ppmdcompressionsettings/
---
## PPMdCompressionSettings(int, int) {#constructor_1}

の新しいインスタンスを初期化します[`PPMdCompressionSettings`](../)class.

```csharp
public PPMdCompressionSettings(int modelOrder, int suballocatorSize)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| modelOrder | Int32 | モデルの順番。 |
| suballocatorSize | Int32 | MB サブアロケータのメモリ サイズが消費される可能性があります。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | *modelOrder*は 2 から 16 の間ではありません。 - または -*suballocatorSize*は 1 から 256 の間ではありません。 |

### 備考

モデルオーダーが大きいほど、ほぼ確実に圧縮率が向上し、メモリと CPU の使用量が確実に増加します。

PPMd アルゴリズムは、特に大きなファイルで使用したり、大きなモデル順序で使用したりする場合に、大量のメモリを必要とする場合があります。

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings(4, 10))))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [PPMdCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* 組み立て [Aspose.Zip](../../../)

---

## PPMdCompressionSettings() {#constructor}

の新しいインスタンスを初期化します[`PPMdCompressionSettings`](../)デフォルトのモデル順序とサブアロケータ サイズを持つクラス.

```csharp
public PPMdCompressionSettings()
```

### 備考

デフォルトのモデル順序は 8 で、サブアロケータのサイズは 50MB です。

### 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new PPMdCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");                   
    archive.Save(zipFile);
}
```

### 関連項目

* class [PPMdCompressionSettings](../)
* 名前空間 [Aspose.Zip.Saving](../../ppmdcompressionsettings/)
* 組み立て [Aspose.Zip](../../../)


