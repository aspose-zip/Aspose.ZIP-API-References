---
title: "CpioArchive.SaveGzipped"
second_title: "Aspose.ZIP .NET 用 API リファレンス"
description: "CpioArchive メソッド。gzip 圧縮でストリームにアーカイブを保存します。"
type: docs
weight: 90
url: /ja/net/aspose.zip.cpio/cpioarchive/savegzipped/
---
## SaveGzipped(Stream, CpioFormat) {#savegzipped}

gzip 圧縮でアーカイブをストリームに保存します。

```csharp
public void SaveGzipped(Stream output, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| output | Stream | 出力ストリーム。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ArgumentNullException | *output* は null です。 |
| ArgumentException | *output* は書き込み可能ではありません。 |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |

## 備考

*output* must be writable.

## 例

```csharp
using (FileStream result = File.OpenWrite("result.cpio.gz"))
{
    using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
    {
        using (var archive = new CpioArchive())
        {
            archive.CreateEntry("entry.bin", source);
            archive.SaveGzipped(result);
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

## SaveGzipped(string, CpioFormat) {#savegzipped_1}

gzip 圧縮でパスで指定されたファイルにアーカイブを保存します。

```csharp
public void SaveGzipped(string path, CpioFormat cpioFormat = CpioFormat.OldAscii)
```

| パラメーター | 型 | 説明 |
| --- | --- | --- |
| path | String | 作成するアーカイブのパス。指定されたファイル名が既存のファイルを指す場合、上書きされます。 |
| cpioFormat | CpioFormat | cpio ヘッダー形式を定義します。 |

### 例外

| 例外 | 条件 |
| --- | --- |
| ObjectDisposedException | アーカイブは破棄されており、使用できません。 |
| ArgumentException | *path* は長さゼロの文字列であるか、空白文字のみを含むか、InvalidPathChars で定義された 1 つ以上の無効な文字を含んでいます。 |
| ArgumentNullException | *path* は `null` です。 |
| DirectoryNotFoundException | 指定されたパスが無効です（例: マッピングされていないドライブ上にある場合）。 |
| IOException | I/O エラーが発生しました。 |
| PathTooLongException | 指定されたパス、ファイル名、またはその両方がシステムで定義された最大長を超えています。 |
| UnauthorizedAccessException | 呼び出し元に必要な権限がありません。-または- *path* が読み取り専用のファイルまたはディレクトリを指定しました。 |

## 例

```csharp
using (FileStream source = File.Open("data.bin", FileMode.Open, FileAccess.Read))
{
    using (var archive = new CpioArchive())
    {
        archive.CreateEntry("entry.bin", source);
        archive.SaveGzipped("result.cpio.gz");
    }
}
```

### 関連項目

* enum [CpioFormat](../../cpioformat/)
* class [CpioArchive](../)
* namespace [Aspose.Zip.Cpio](../../cpioarchive/)
* assembly [Aspose.Zip](../../../)


