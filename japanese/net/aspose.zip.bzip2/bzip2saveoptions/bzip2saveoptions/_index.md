---
title: "Bzip2SaveOptions.Bzip2SaveOptions"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "Bzip2SaveOptions コンストラクタ。Bzip2SaveOptions クラスの新しいインスタンスを初期化します。"
type: docs
weight: 10
url: /ja/net/aspose.zip.bzip2/bzip2saveoptions/bzip2saveoptions/
---
## Bzip2SaveOptions(int) {#constructor_1}

[`Bzip2SaveOptions`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Bzip2SaveOptions(int blockSize)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| blockSize | Int32 | ブロックサイズ（百キロバイト単位）。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentOutOfRangeException | ブロックサイズが有効な範囲ではありません。 |

## 例

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
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)

---

## Bzip2SaveOptions() {#constructor}

デフォルトのブロックサイズ（9 百キロバイト）で、[`Bzip2SaveOptions`](../) クラスの新しいインスタンスを初期化します。

```csharp
public Bzip2SaveOptions()
```

## 例

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
* namespace [Aspose.Zip.Bzip2](../../bzip2saveoptions/)
* assembly [Aspose.Zip](../../../)


