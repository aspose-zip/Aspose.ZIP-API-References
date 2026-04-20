---
title: Bzip2SaveOptions.Bzip2SaveOptions
second_title: Aspose.ZIP for .NET API リファレンス
description: Bzip2SaveOptions コンストラクタ. の新しいインスタンスを初期化しますBzip2SaveOptionsclass.
type: docs
weight: 10
url: /ja/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

の新しいインスタンスを初期化します[`Bzip2SaveOptions`](../)class.

```csharp
public Bzip2SaveOptions(int blockSize)
```

| パラメータ | タイプ | 説明 |
| --- | --- | --- |
| blockSize | Int32 | 数百キロバイト単位のブロック サイズ。 |

### 例外

| 例外 | 調子 |
| --- | --- |
| ArgumentOutOfRangeException | ブロック サイズが有効な範囲にありません。 |

### 例

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions(9));
    }
}
```

### 関連項目

* class [Bzip2SaveOptions](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* 組み立て [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

の新しいインスタンスを初期化します[`Bzip2SaveOptions`](../)デフォルトのブロック サイズを持つクラスで、900 キロバイトに相当します。

```csharp
public Bzip2SaveOptions()
```

### 例

```csharp
using (FileStream result = File.Open("archive.bz2"))
{
    using (Bzip2Archive archive = new Bzip2Archive())
    {
        archive.SetSource("data.bin");
        archive.Save(result, new Bzip2SaveOptions());
    }
}
```

### 関連項目

* class [Bzip2SaveOptions](../)
* 名前空間 [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* 組み立て [Aspose.Zip](../../../)


