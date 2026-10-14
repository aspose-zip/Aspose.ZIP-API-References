---
title: "LzmaCompressionSettings.LzmaCompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "LzmaCompressionSettings コンストラクタ。デフォルトパラメータで LzmaCompressionSettings クラスの新しいインスタンスを初期化します"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/lzmacompressionsettings/lzmacompressionsettings/
---
## LzmaCompressionSettings() {#constructor}

デフォルトパラメータで [`LzmaCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public LzmaCompressionSettings()
```

## 例

```csharp
using (Archive archive = new Archive(new ArchiveEntrySettings(new LzmaCompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save(zipFile);
}
```

### 関連項目

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int, int, int) {#constructor_2}

指定された辞書サイズ、ファストバイト数、リテラルコンテキストビット数で [`LzmaCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public LzmaCompressionSettings(int dictionarySize, int numberOfFastBytes, int literalContextBits)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 辞書（履歴バッファ）のサイズ（バイト単位）。4096 から 1073741824 の範囲で指定する必要があります。 |
| numberOfFastBytes | Int32 | LZMA アルゴリズムにおける高速マッチ検索に使用されるバイト数。5 から 273 の範囲で指定できます。 |
| literalContextBits | Int32 | リテラルコンテキストビット数（前のリテラルの上位ビット）を設定します。範囲は0から8までです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | 引数のいずれかが許容範囲外の場合にスローされます。 |

### 関連項目

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## LzmaCompressionSettings(int) {#constructor_1}

指定された辞書サイズ、デフォルトの高速バイト数が32、リテラルコンテキストビット数が3で、[`LzmaCompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public LzmaCompressionSettings(int dictionarySize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 辞書（履歴バッファ）のサイズ（バイト単位）。4096 から 1073741824 の範囲で指定する必要があります。 |

### 関連項目

* class [LzmaCompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../lzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


