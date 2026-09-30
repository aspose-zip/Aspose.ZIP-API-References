---
title: "SevenZipLZMACompressionSettings.SevenZipLZMACompressionSettings"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "SevenZipLZMACompressionSettings コンストラクタ。デフォルトパラメータで SevenZipLZMACompressionSettings クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.saving/sevenziplzmacompressionsettings/sevenziplzmacompressionsettings/
---
## SevenZipLZMACompressionSettings() {#constructor}

[`SevenZipLZMACompressionSettings`](../) クラスの新しいインスタンスをデフォルトパラメータで初期化します。

```csharp
public SevenZipLZMACompressionSettings()
```

## 例

```csharp
using (var archive = new SevenZipArchive(new SevenZipEntrySettings(new SevenZipLZMACompressionSettings())))
{
    archive.CreateEntry("data.bin", "data.bin");
    archive.Save("result.7z");
}
```

### 関連項目

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int, int, int) {#constructor_2}

指定された辞書サイズ、ファストバイト数、リテラルコンテキストビット数で、[`SevenZipLZMACompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize, int numberOfFastBytes, 
    int literalContextBits)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 辞書（履歴バッファ）のサイズ（バイト単位）。4096 から 1073741824 の間である必要があり、エントリサイズに基づく自動検出の場合は 0 に設定できます。 |
| numberOfFastBytes | Int32 | LZMA アルゴリズムにおける高速マッチ検索に使用されるバイト数。5 から 273 の範囲で指定できます。 |
| literalContextBits | Int32 | リテラルコンテキストビット数（前のリテラルの上位ビット）を設定します。範囲は0から8までです。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | 引数のいずれかが許容範囲外の場合にスローされます。 |

### 関連項目

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)

---

## SevenZipLZMACompressionSettings(int) {#constructor_1}

辞書サイズ、ファストバイト数を 32、リテラルコンテキストビット数を 3 に指定して、[`SevenZipLZMACompressionSettings`](../) クラスの新しいインスタンスを初期化します。

```csharp
public SevenZipLZMACompressionSettings(int dictionarySize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| dictionarySize | Int32 | 辞書（履歴バッファ）のサイズ（バイト単位）。4096 から 1073741824 の間である必要があり、エントリサイズに基づく自動検出の場合は 0 に設定できます。 |

### 関連項目

* class [SevenZipLZMACompressionSettings](../)
* namespace [Aspose.Zip.Saving](../../sevenziplzmacompressionsettings/)
* assembly [Aspose.Zip](../../../)


