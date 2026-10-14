---
title: "CpioArchive.SaveLZMACompressed"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CpioArchive メソッド。LZMA 圧縮でアーカイブをストリームに保存します"
type: docs
weight: 110
url: /ja/net/aspose.zip.cpio/cpioarchive/savelzmacompressed/
---
## SaveLZMACompressed(Stream, CpioFormat) {#savelzmacompressed}

LZMA 圧縮でアーカイブをストリームに保存します。

```csharp
public void SaveLZMACompressed(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| NotSupportedException | ストリームは書き込みをサポートしていないか、既に閉じられています。 |

## 備考

*output* must be writable.

重要: cpio アーカイブはこのメソッド内で構成され、その後圧縮され、内容は内部に保持されます。メモリ使用量に注意してください。

## 例

```csharp
using (FileStream result = File.OpenWrite("result.cpio.lzma"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveLZMACompressed(result);
        }
    }
}
```

### 関連項目

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)

---

## SaveLZMACompressed(string, CpioFormat) {#savelzmacompressed_1}

lzma 圧縮でパスで指定したファイルにアーカイブを保存します。

```csharp
public void SaveLZMACompressed(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentNullException | *path* は `null` です。 |
| 例外 | 実行時エラーが発生したときにスローされます。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | I/O エラーが発生しました。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | 呼び出し元に必要な権限がありません。-または- *path* が読み取り専用のファイルまたはディレクトリを指定しました。 |

## 備考

重要: cpio アーカイブはこのメソッド内で構成され、その後圧縮され、内容は内部に保持されます。メモリ使用量に注意してください。

## 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveLZMACompressed("result.cpio.lzma");
    }
}
```

### 関連項目

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


